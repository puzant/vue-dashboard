<template lang="pug">
  .tasks-container
    .tasks-text
      | MY TASKS

    .add-tasks-container
        input.input-tasks( placeholder="Enter a new Task" v-model="task")
        button.add-task-btn( @click="addNewTasks" ) ADD TASK

    .list-of-tasks-container
      .task(v-for="(task, index) in tasks")
        .task-content
          input( type="checkbox" )
          .listed-task-text {{task}}
        .delete-task( click="deleteTask" )
          img(src="@/assets/delete.svg")

</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'
@Component({})
export default class Tasks extends Vue {
  tasks = ['Create chart to regional sales', 'Contact John from HR', 'Prepare for meeting', 'Contact Reachel from PR', 'plane for presentation']
  task: string = ''

  addNewTasks() {
    let newTask = this.task
    this.tasks.push(this.task)
    this.task = ''
  }

  deleteTask() {

  }

}
</script>

<style lang="sass">
.tasks-container
  margin-top: 20px
  margin-left: -35px
  border-radius: 5px
  width: 320px
  height: 589px
  background-color: #212936
  padding: 20px
  box-shadow: 0px 6px 10px rgba(0, 0, 0, 0.14), 0px 1px 18px rgba(0, 0, 0, 0.12), 0px 3px 5px rgba(0, 0, 0, 0.2)

.tasks-text
  color: #8997B1
  font-weight: 500

.add-tasks-container
  display: flex
  flex-direction: row
  margin-top: 10px

.input-tasks
  padding: 10px
  border-radius: 5px
  border: 1px solid #56657F
  background: none
  color: #fff
  width: 73%
  box-shadow: 0px 6px 10px rgba(0, 0, 0, 0.14), 0px 1px 18px rgba(0, 0, 0, 0.12), 0px 3px 5px rgba(0, 0, 0, 0.2)
  &:focus
    outline: none

.list-of-tasks-container
  margin-top: 30px

.add-task-btn
  background-color: #1976D2
  border: none
  border-radius: 5px
  color: #fff
  width: 70px
  font-weight: 500
  font-size: 10px
  margin-left: 10px
  box-shadow: 0px 6px 10px rgba(0, 0, 0, 0.14), 0px 1px 18px rgba(0, 0, 0, 0.12), 0px 3px 5px rgba(0, 0, 0, 0.2)
  &:focus
    outline: none
  &:hover
    cursor: pointer

.task
  display: flex
  justify-content: space-between
  align-items: center
  // width: 97%
  margin-top: 10px
  color: #8997B1

.task-content
  display: flex
  align-items: center

.listed-task-text
  margin-left: 4px

.delete-task
  &:hover
    cursor: pointer

.delete-task img
  width: 15px
  display: flex
</style>