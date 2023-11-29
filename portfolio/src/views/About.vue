<script>
export default {};
</script>

<template>
  <div class="d-flex justify-content-center mt-5">

    <div class="card green">

        <div >
            <img class="card-img" src="../assets/images/women_avatar.png" width="70" height="100"/>
        </div>
             
          <div class="additional">
            
            <div class="more-info">
              <h1>Jane Doe</h1>
              <div class="coords">
                <span>Group Name</span>
                <span>Joined January 2019</span>
              </div>
              <div class="coords">
                <span>Position/Role</span>
                <span>City, Country</span>
              </div>
              
            </div>
          </div>
          <div class="general">
            <h1>Ruhi R. Ambelkar</h1>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce a
              volutpat mauris, at molestie lacus. Nam vestibulum sodales odio ut
              pulvinar.
            </p>
            
          </div>
        </div>
  </div>
</template>

<style scoped>

.card-img {
    position: absolute;
    /* border-radius: 50%; */
    /* border: 5px black solid; */
    padding: 9px 4px;
    z-index: 99999999;
    display: flex;
    justify-content: left;
    width: 33%;
}
.card {
  width: 450px;
  height: 250px;
  background-color: #fff;
  background: linear-gradient(#f8f8f8, #fff);
  box-shadow: 0 8px 16px -8px rgba(0, 0, 0, 0.4);
  border-radius: 30px;
  overflow: hidden;
  position: relative;
  margin: 1.5rem;
}

.card h1 {
  text-align: center;
}

.card .additional {
  position: absolute;
  width: 150px;
  height: 100%;
  
  transition: width 0.4s;
  overflow: hidden;
  z-index: 2;
}

.card.green .additional {
  background: linear-gradient(rgb(4, 46, 49),rgb(4, 46, 49));
}

.card:hover .additional {
  width: 100%;
  border-radius: 0 30px 30px 0;
}

.card .additional .more-info {
  width: 300px;
  float: left;
  position: absolute;
  left: 150px;
  height: 100%;
}

.card .additional .more-info h1 {
  color: #fff;
  margin-bottom: 0;
}

.card.green .additional .more-info h1 {
  color: #ffffff;
}

.card .additional .coords {
  margin: 0 1rem;
  color: #fff;
  font-size: 1rem;
}

.card.green .additional .coords {
  color: #ffffff;
}

.card .additional .coords span + span {
  float: right;
}






.card .general {
  width: 300px;
  height: 100%;
  position: absolute;
  top: 0;
  right: 0;
  z-index: 1;
  box-sizing: border-box;
  padding: 1rem;
  padding-top: 0;
}

.card .general .more {
  position: absolute;
  bottom: 1rem;
  right: 1rem;
  font-size: 0.9em;
}
</style>
