<template lang="pug">
  .client-messages-container
    .messages-text
      | Messages

    .messages-list-container

      .message
        img.message-logo(src="@/assets/info.svg")
        .message-text-date-container
          .message-date
            | 1/1/2020
          .message-text
          | Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut ali


      .message
        img.message-logo(src="@/assets/info.svg")
        .message-text-date-container
          .message-date
            | 1/1/2020
          .message-text
            | Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.


        
      

</template>


<style lang="sass">
.client-messages-container
  overflow: scroll
  width: 718px
  height: 334px
  background-color: #212936
  padding: 20px
  margin-top: 20px
  margin-left: 10px
  box-shadow: 0px 6px 10px rgba(0, 0, 0, 0.14), 0px 1px 18px rgba(0, 0, 0, 0.12), 0px 3px 5px rgba(0, 0, 0, 0.2)

.messages-list-container
  margin-top: 28px

.message
  border: 1px solid #3b3b3b
  border-radius: 5px
  display: flex
  flex-direction: row
  align-items: center
  margin: 10px
  padding: 10px

.messages-text
  color: #AFBDD1
  font-size: 20px
  font-weight: 500
  margin: 5px 0 0 0

.message-logo
  height: 30px

.message-text-date-container
  margin-left: 10px
</style>