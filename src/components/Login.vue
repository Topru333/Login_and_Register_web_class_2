<template>
  <div class="login">
    <div class="main-form">
      <i class="logo"></i>
      <input type="text" placeholder="Username" value="" />
      <input type="password" placeholder="Password" value="" />
      <input type="submit" value="Sign in" />
      <div><a href="#" title="">Sign Up</a></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Login",
  props: {
    msg: String
  }
};
</script>

<style scoped>
* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
body {
  background: url(http://i.imgur.com/MQB99sg.jpg) #a9b89e;
  font-family: Arial;
  font-size: 12px;
  color: #c4bcb0;
}
input[type="text"],
input[type="password"],
input[type="submit"] {
  background: #eae6e1;
  border: 0;
  font-weight: bold;
  padding: 10px;
  border-radius: 3px;
  width: 100%;
  margin: 5px 0;
  outline: medium none;
  color: #838383;
}
input[type="checkbox"] {
  -webkit-appearance: none;
  width: 10px;
  height: 10px;
  position: relative;
  outline: medium none;
  margin-right: 10px;
}
input[type="checkbox"]::before {
  width: 9px;
  height: 9px;
  content: "";
  display: block;
  border: 3px solid #c4bcb0;
  border-radius: 9px;
  position: absolute;
}
input[type="checkbox"]:checked::after {
  width: 5px;
  height: 5px;
  content: "";
  display: block;
  background: #c4bcb0;
  border-radius: 5px;
  position: absolute;
  left: 5px;
  top: 5px;
}
input[type="submit"] {
  display: block;
  padding: 10px;
  background: #50bfa4;
  border: 0;
  border-radius: 3px;
  width: 100%;
  color: #fff;
  cursor: pointer;
  -webkit-transition: all 0.3s;
  -moz-transition: all 0.3s;
  transition: all 0.3s;
}
input[type="submit"]:hover {
  background: #58ccb0;
}
.main-form {
  width: 350px;
  margin: 100px auto;
  padding: 50px;
  border: 1px solid rgba(0, 0, 0, 0.1);
  -webkit-box-shadow: 0 1px 2px rgba(0, 0, 0, 0.2);
  background: #fff;
}
.logo {
  background: #50bfa4;
  width: 40px;
  height: 40px;
  display: block;
  margin: 0 auto 30px;
  border-top-left-radius: 20px;
  border-top-right-radius: 20px;
  border-bottom-left-radius: 20px;
  position: relative;
  -webkit-transform: rotate(45deg);
  -moz-transform: rotate(45deg);
  transform: rotate(45deg);
}
.logo::before {
  width: 14px;
  height: 14px;
  display: block;
  border: 5px solid #f7f5f2;
  content: "login";
  position: absolute;
  border-radius: 14px;
  top: 8px;
  left: 8px;
}
.main-form > label {
  display: block;
  margin: 10px 0 15px;
  line-height: 15px;
  cursor: pointer;
}
.main-form > div {
  margin-top: 20px;
}

.main-form > div > a:first-child {
  font-weight: bold;
}
.main-form > div > a:nth-child(1) {
  border: 1px solid #3da087;
  display: inline-block;
  text-decoration: none;
  border-radius: 3px;
  color: #3da087;
  font-weight: bold;
  padding: 7px 15px;
  -webkit-transition: all 0.3s;
  -moz-transition: all 0.3s;
  transition: all 0.3s;
}
.main-form > div > a:nth-child(1):hover {
  background: #3da087;
  color: #fff;
}
</style>
