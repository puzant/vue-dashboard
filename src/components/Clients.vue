<template lang="pug">
  .clients-container
    .new-clients-text
      | New Clients

    .new-client-info-container
      .new-client-image-name
        .client-image
          img( src="@/assets/client-1.svg" )
        .client-name-country
          .client-name Nicci Troani 
          .client-country Chicago, IL
      .client-menu
        img( src="@/assets/menu.svg" )

    .new-client-info-container
      .new-client-image-name
        .client-image
          img( src="@/assets/client-2.svg" )
        .client-name-country
          .client-name George Feilds 
          .client-country New York, NY
      .client-menu
        img( src="@/assets/menu.svg" )
    
    .new-client-info-container
      .new-client-image-name
        .client-image
          img( src="@/assets/client-3.svg" )
        .client-name-country
          .client-name Nicci Troani 
          .client-country Chicago, IL
      .client-menu
        img( src="@/assets/menu.svg" )

    .new-client-info-container
      .new-client-image-name
        .client-image
          img( src="@/assets/client-4.svg" )
        .client-name-country
          .client-name Nicci Troani 
          .client-country Chicago, IL
      .client-menu
        img( src="@/assets/menu.svg" )

</template>


<style lang="sass">
.clients-container
  margin-left: 266px
  margin-top: 20px
  height: 334px
  overflow: scroll
  width: 340px
  border-radius: 5px
  padding: 20px
  background-color: #212936

.new-clients-text
  color: #AFBDD1
  font-size: 20px
  font-weight: 500
  // padding: 20px
  margin-top: 20px

.new-client-info-container
  width: 95%
  display: flex
  flex-direction: row
  justify-content: space-between
  align-items: center
  margin-top: 20px

.new-client-image-name
  display: flex
  flex-direction: row

.client-name-country
  margin-left: 10px

.client-name
  color: #8997B1
  font-size: 18px

.client-country
  color: #56657F
  font-size: 14px

.client-menu
  &:hover
    cursor: pointer
</style>