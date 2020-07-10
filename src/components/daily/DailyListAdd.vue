<template>
  <div class="daily-list-add">
    <form class="add-cont">
      <ul>
        <li class="add-income">
          <a href="#/daily">수입</a>
          <button class="btn what-date">7월10일</button>
          <select name="" id="">
            <option selected>분류1</option>
            <option>분류2</option>
            <option>분류3</option>
          </select>
          <select name="" id="" class="add-bank">
            <option selected>은행1</option>
            <option>은행2</option>
            <option>은행3</option>
          </select>
          <input
            type="text"
            placeholder="내역을 0 단위로 입력해주세요. ex 10,000"
          />
          <button class="btn list-add-btn">등록</button>
        </li>
        <li class="add-expend">
          <a href="#/daily">지출</a>
          <!-- <button class="btn what-date">7월10일</button>
          <select name="" id="">
            <option selected>분류1</option>
            <option>분류2</option>
            <option>분류3</option>
          </select>
          <select name="" id="" class="add-bank">
            <option selected>은행1</option>
            <option>은행2</option>
            <option>은행3</option>
          </select>
          <input
            type="text"
            placeholder="내역을 0 단위로 입력해주세요. ex 10,000"
          />
          <button class="btn list-add-btn">등록</button> -->
        </li>
      </ul>
    </form>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
