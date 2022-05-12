<template>
    <div>
        <b-container>
            <div class="list-card">
            <b-row class="content">
                <b-col cols="4" class="message-div">
                    <div class="message_box">
                <h5>You Have 5 New Messages</h5>
                <div class="list-group rounded-0">
                  <a class="list-group-item list-group-item-action active text-white rounded-0">
                    <div class="media icon-container">
                      <img src="https://www.mockofun.com/wp-content/uploads/2019/12/circle-profile-pic.jpg" alt="user" width="50">
                      <div class='status-circle'>
                      </div>
                      <div class="media-body">
                        <div class="d-inline-flex align-items-center justify-content-between mb-1">
                          <h6 class="mb-0">Jason Doe</h6>
                        </div>
                        <p class="font-italic mb-0 text-small">Like my new protfolio.</p>
                        <div class="right"><button type="button" class="btn btn-primary btn-sm"> Add</button></div>
                      </div>
                    </div>
                  </a>
                  <a class="list-group-item list-group-item-action active text-white rounded-0">
                    <div class="media icon-container">
                      <img src="https://www.mockofun.com/wp-content/uploads/2019/12/circle-photo.jpg" alt="user" width="50">
                      <div class='status-circle'>
                      </div>
                      <div class="media-body">
                        <div class="d-inline-flex align-items-center justify-content-between mb-1">
                          <h6 class="mb-0">Jason Doe</h6>
                        </div>
                        <p class="font-italic mb-0 text-small">I have sing a song.</p>
                        <div class="right"><button type="button" class="btn btn-primary btn-sm"> Add</button></div>
                      </div>
                    </div>
                  </a>
                  <a class="list-group-item list-group-item-action active text-white rounded-0">
                    <div class="media icon-container">
                      <img src="https://www.pngitem.com/pimgs/m/75-758282_walter-circle-person-photo-in-circle-hd-png.png" alt="user" width="50">
                      <div class='circle_red'>
                      </div>
                      <div class="media-body">
                        <div class="d-inline-flex align-items-center justify-content-between mb-1">
                          <h6 class="mb-0">Jason Doe</h6>
                        </div>
                        <p class="font-italic mb-0 text-small">Just design new Dribble.</p>
                        <div class="right"><button type="button" class="btn btn-primary btn-sm"> Add</button></div>
                      </div>
                    </div>
                  </a>
                </div>
              </div>
                </b-col>
                  <b-col cols="4" class="message-div">
                     <div class="check_box">
                <h5>To Do List</h5>
                <form class="check">
                  <b-form-group>
                    <input type="checkbox" id="html">
                    <label for="html">Schedule Meeting</label>
                  </b-form-group>
                   <b-form-group>
                    <input type="checkbox" id="css">
                    <label for="css">Call clients for follow_up<button class="red">Today</button></label>
                   </b-form-group>
                  <b-form-group>
                    <input type="checkbox" id="javascript">
                    <label for="javascript">Book flight for holiday</label>
                  </b-form-group>
                  <div class="form-group">
                    <input type="checkbox" id="html">
                    <label for="html">Forward important tasks<button class="blue">2 week</button></label>
                  </div>
                  <b-form-group>
                    <input type="checkbox" id="css">
                    <label for="css">Receive shipment</label>
                  </b-form-group>
                 <b-form-group>
                    <input type="checkbox" id="javascript">
                    <label for="javascript">Important task</label>
                 </b-form-group>
                </form>
              </div>
                  </b-col>
                    <b-col cols="4" class="message-div">
                         <div class="card_profile">
                <div class="profile-card-img">
                  <img class="card-img-top"
                    src="https://s3.eu-central-1.amazonaws.com/bootstrapbaymisc/blog/24_days_bootstrap/oslo.jpg"
                    alt="Bologna">

                  <img class="avatar rounded-circle" src="https://www.pngitem.com/pimgs/m/75-758282_walter-circle-person-photo-in-circle-hd-png.png">
                </div>
                <div class="card-body text-center">
                  <h4 class="card-title">Septiandika Pratama</h4>
                  <h6 class="card-subtitle text-muted">Graphics Designer</h6>
                  <p class="card-text">Lorem ipsum dolor,sit amet consectetur adipisicing elit. Enim quidem, repellendus
                    natus! </p>
                  <div class="profile-card-inf">
                    <div class="profile-card-inf__item">
                      <div class="profile-card-inf__title">1598</div>
                      <div class="profile-card-inf__txt">Followers</div>
                    </div>

                    <div class="profile-card-inf__item">
                      <div class="profile-card-inf__title">65</div>
                      <div class="profile-card-inf__txt">Following</div>
                    </div>

                    <div class="profile-card-inf__item">
                      <div class="profile-card-inf__title">123</div>
                      <div class="profile-card-inf__txt">Articles</div>
                    </div>
                  </div>
                </div>
              </div>
                    </b-col>
            </b-row>
            </div>
        </b-container>
    </div>
</template>
<script>
export default {
    name:"list-page"
}
</script>
<style scoped>
.list-card{
    margin-top: 20px;

}
.profile-card-inf {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    align-items: flex-start;
}
.profile-card-inf__item {
    padding: 10px 5px;
    min-width: 90px;
    margin-top: 5px;
}
.profile-card-inf__title {
    font-weight: 500;
    font-size: 16px;
    color: #111213;
}
.profile-card-inf__txt {
    font-weight: 300;
    font-size: 12px;
    margin-top: 3px;
    color: #727171;
}
.red {
    background-color: #243657;
    color: white;
    border: none;
    border-radius: 3px;
    margin-left: 10px;
}
.blue {
    background-color: #243657;
    color: white;
    border: none;
    border-radius: 3px;
    margin-left: 10px;
}
.message_box {
  background-color: white;
  padding-bottom: 12px;
 box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0 6px 6px rgba(0,0,0,0.23);;
  transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
  border-radius: 0.375rem;
}
.message_box h5 {
  padding-top: 12px;
  padding-left: 30px;
  font-size: 19px;
}

.avatar {
  border: 0.3rem solid rgba(#fff, 0.3);
  max-width: 7rem;
}
.profile-card-img {
  position: relative;
  top: 0;
  left: 0;
}
.avatar {
  position: absolute;
  top: 12%;
  left: 35%;
}
.rounded-circle {
  border-radius: 50% !important;
}
.card-body {
  padding: 0 !important;
  margin-top: 20px;
}
.card-img-top {
  width: 100%;
  height: 160px;
  object-fit: cover;
}
.card-title {
  font-size: 20px;
  font-weight: 700;
}
.card-subtitle {
  font-size: 15px;
}
.card-text {
  font-size: 14px;
  padding: 10px;
}
.card_profile {
  background-color: #fff;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
  transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
  border-radius: 0.375rem;
      padding-bottom: 10px;
}
.list-group-item.active {
  background-color: white !important;
  padding-top: 20px;
  border: none !important;
  color: black !important;
}
.check_box {
    background-color: white;
    padding-left: 30px;
    padding-bottom: 40px;
     box-shadow: 0 14px 28px rgba(0,0,0,0.25), 0 10px 10px rgba(0,0,0,0.22);
    transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
     border-radius: 0.375rem;
}
.check_box h5{
    padding-top: 15px;
}
.check{
    padding-top: 10px;
}
.right {
    flex: 0 0 auto;
    width: auto;
    max-width: 100%;
}
@media (max-width: 1024px){
.check_box {
    padding-left: 25px;
    padding-bottom: 55px;
}
.message_box[data-v-571e590e] {
    padding-bottom: 28px;
}
}
@media (max-width: 800px){
  .avatar {
    position: absolute;
    top: 12%;
    left: 25%;
}
}
@media (max-width: 640px){
  .check_box {
    padding-bottom: 59px ;
    }
    .message_box {
    padding-bottom: 12px;
    }
    .card_profile {
    padding-bottom: 47px;
    }
}
 @media (max-width: 640px){
    .message_box {
    padding-bottom: 10px !important;
    }
    .check_box {
    padding-bottom: 45px;
    }
    .card_profile {
    padding-bottom: 32px;
    }
    .icon {
    margin-left: 0px !important;
        font-size: 1.8rem;
    }
    .avatar {
    left: 12% !important;
    }
}
  @media (max-width: 580px){
 .avatar {
    left: 12% !important;
 }
  }
  @media (max-width: 460px){
.avatar {
    left: 5% !important;
}
.text-muted{
    font-size: 13px;
}
.check_box {
    padding-bottom: 15px;
}
.message_box {
    padding-bottom: 75px !important;
}
.card_profile{
    padding-bottom: 75px;
}
  }
    @media (max-width: 480px){
.check_box{
    padding-left: 35px;
    }
    .avatar {
    left: 37% !important;
    }
    }
    @media (max-width: 360px){
.check_box {
    padding-left: 10px;
}
    }
@media screen and (min-device-width: 320px) and (max-device-width: 640px) { 
  .content{
    flex-direction: column;
  }
  .check_box {
  margin-top: 12px;
}
.message_box {
    margin-top: 12px;
}
.card_profile{
    margin-top: 12px;
}
.message-div{
  max-width: 100%;
}
}
</style>