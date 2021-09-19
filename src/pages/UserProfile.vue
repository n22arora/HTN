<template>
    <div class="row">
      <div class="col-xl-4 col-lg-5 col-md-4">
        <profile-1></profile-1>
        <profile-4></profile-4>
      </div>
      <div class="col-xl-4 col-lg-5 col-md-4">
        <profile-2></profile-2>
        <profile-5></profile-5>        
      </div>
      <div class="col-xl-4 col-lg-5 col-md-4">
        <profile-3></profile-3>
        <profile-6></profile-6>

      </div>
    </div>
</template>
<script>
import EditProfileForm from "./UserProfile/EditProfileForm.vue";
import UserCard from "./UserProfile/UserCard.vue";
import MembersCard from "./UserProfile/MembersCard.vue";
import Profile1 from './UserProfile/Profile1.vue';
import Profile2 from './UserProfile/Profile2.vue';
import Profile3 from './UserProfile/Profile3.vue';
import Profile4 from './UserProfile/Profile4.vue';
import Profile5 from './UserProfile/Profile5.vue';
import Profile6 from './UserProfile/Profile6.vue';
export default {
  components: {
    EditProfileForm,
    UserCard,
    MembersCard,
    Profile1,
    Profile2,
    Profile3,
    Profile4,
    Profile5,
    Profile6
  }
};
</script>
<style>
</style>
