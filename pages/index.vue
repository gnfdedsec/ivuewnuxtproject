<template lang="html">
  <div align="center">
    <div class="wrap">
      <p>ค้นหา</p>

      <div class="search">
        <input
          type="text"
          class="searchTerm"
          placeholder="ex : เลขที่ประกาศ ,เลขที่คำสั่ง "
        />
        <button type="submit" class="searchButton">
          <font-awesome-icon :icon="['fas', 'search']" />
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
p {
  font-family: kanit;
  font-size: 24px;
}
.search {
  width: 100%;
  position: relative;
  display: flex;
}

.searchTerm {
  width: 100%;
  border: 1px solid #00b4cc;
  border-right: none;
  padding: 5px;
  height: 36px;
  border-radius: 5px 0 0 5px;
  outline: none;
  color: #9dbfaf;
  font-family: kanit;
}

.searchTerm:focus {
  color: #080808;
}

.searchButton {
  width: 50px;
  height: 36px !important;
  border: 1px solid #00b4cc;
  background: #00b4cc;
  text-align: center;
  color: #fff;
  border-radius: 0 5px 5px 0;
  cursor: pointer;
  font-size: 15px;
}

/*Resize the wrap to see the search bar change!*/
.wrap {
  width: 30%;
  position: absolute;
  top: 5%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>
