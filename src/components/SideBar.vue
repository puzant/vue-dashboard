<template lang="pug">
  .side-bar-container

    .side-bar-content

      .user-avatar-container
        img(src="@/assets/user.svg")
      .user-name-container
        .user-name
          | Aaron Young  
        .dropdown-icon
          img(src="@/assets/arrow_drop_down.svg")

    .separator

      .dashboard-controls
        .dashboard-btn
          img(src="@/assets/dashboard.svg")
          span.btn-text Dashbaoard

        .dashboard-btn
          img(src="@/assets/message.svg")
          span.btn-text Messages

        .dashboard-btn
          img(src="@/assets/assignment.svg")
          span.btn-text My Tasks

        .dashboard-btn
          img(src="@/assets/clients.svg")
          span.btn-text Clients
        
    .separator

      .settings-container
        .settings-text  Settings

      .dashboard-btn
          img(src="@/assets/settings.svg")
          span.btn-text Main Settings

      .dashboard-btn
          img(src="@/assets/integration.svg")
          span.btn-text Integrations

</template>




<style lang="sass">
.side-bar-container
  width: 255px
  height: 100%
  position: fixed
  top: 0
  left: 0
  background-color: #212936

.side-bar-content
  margin-left: 20px

.user-avatar-container
  margin: 50px 0 0 0

.user-name-container
  display: flex
  justify-content: space-between
  align-items: flex-end

.dropdown-icon
  margin-right: 10px
  margin-top: 17px

.user-name
  color: #AFBDD1
  font-size: 20px
  font-weight: 500
  margin-top: 20px

.separator
  border-top: 1px solid #313C4E
  margin-top: 20px


.dashboard-btn
  width: 80%
  display: flex
  align-items: center
  transition: .5s
  border-radius: 5px
  margin: 10px auto
  padding: 10px
  &:hover
    background-color: #2B3648
    cursor: pointer
    color: #2B3648

.btn-text
  color: #56657F
  font-weight: 500
  font-size: 14px
  margin-left: 30px

.settings-container
  margin-top: 15px

.settings-text
  color: #56657F
  font-size: 14px
  margin-left: 20px
</style>