<template>
  <div class='nav-two'>
    <div>
      <div>
        <a @click="$router.go(-1)"><i class="fas main-l fa-arrow-left"></i></a>
      </div>
      <div>
      </div>
    </div>
  </div>

</template>
<style scoped>
.nav-two {
  position: sticky;
  top: -1px;
  background: ##205461;
  border-radius: 0% 0% 10% 10%;
  z-index: 10;
}

.nav-two div {
  display: flex;
  justify-content: space-between;
  flex-direction: row;
}

.nav-two a {
  text-decoration: none;
  cursor: pointer;
  margin: 0 14px 0 6px;
  font-size: 1.2em;
}

.nav-two i {
  color: #dbd1d1;
  margin-top: 8px;
  display: flex;
  justify-content: flex-end;
}
</style>
