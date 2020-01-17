<template lang="pug">
  .notifications-container

    .clients-box-container
      img.notification-logo(src="@/assets/people.svg")
      .number-of-clients 128
      .clients-text Clients

    .clients-box-container
      img.notification-logo(src="@/assets/task.svg")
      .number-of-clients 32
      .clients-text Completed tasks

    .clients-box-container
      img.notification-logo(src="@/assets/notifiation.svg")
      .number-of-clients 2
      .clients-text Notifications
    
    .clients-box-container
      img.notification-logo(src="@/assets/warning.svg")
      .number-of-clients 4
      .clients-text reports
</template>


<style lang="sass">
.notifications-container
  display: flex
  margin-left: 255px
  margin-top: 20px
  width: 72%

.number-of-clients
  color: #8997B1
  font-size: 24px


.clients-text
  color: #56657F


.clients-box-container
  margin-left: 10px
  text-align: center
  background-color: #212936
  border: 1px solid #313C4E
  border-radius: 4px
  width: 156px
  height: 120px
  padding: 20px
  display: flex
  flex-direction: column
  justify-content: space-around
  transition: .5s
  &:hover
    border: 1px solid #c1c1c1
    color: #fff
    background-color: #2B3648
    cursor: pointer
    box-shadow: 0px 6px 10px rgba(0, 0, 0, 0.14), 0px 1px 18px rgba(0, 0, 0, 0.12), 0px 3px 5px rgba(0, 0, 0, 0.2)


</style>