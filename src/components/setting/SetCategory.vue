<template>
  <div class="set-category">
    <!-- 수입/지출 카테고리 아이콘 수정 -->
    <div class="category-list-cont">
      <h3 class="font-jua">수입 / 지출 카테고리</h3>
      <form action="">
        <ul>
          <!-- script를 작성하면 li의 '관리비'등의 이름을 {{}}로 줘서 data랑 연동되도록 하면 되겠다 -->
          <li>
            <label
              ><input type="radio" name="category" />
              <!-- 추후에 span 옆에 선택한 아이콘도 넣어줄 것 -->
              <div>
                <i class="fas fa-wallet"></i>
                <span>관리비</span>
                <!-- <img src="../../assets/images/045-ecology.png" alt="" /> -->
              </div>
              <button>✕</button>
            </label>
          </li>
          <li>
            <label
              ><input type="radio" name="category" />
              <div>
                <i class="fas fa-shopping-cart"></i>
                <span>쇼핑</span>
                <!-- <img src="../../assets/images/049-online shopping.png" alt="" /> -->
              </div>
              <button>✕</button>
            </label>
          </li>
          <li>
            <label
              ><input type="radio" name="category" />
              <div>
                <i class="fas fa-utensils"></i>
                <span>식비</span>
                <!-- <img src="../../assets/images/030-cutlery.png" alt="" /> -->
              </div>
              <button>✕</button>
            </label>
          </li>
          <li>
            <label
              ><input type="radio" name="category" />
              <div>
                <i class="fas fa-gas-pump"></i>
                <span>주유비</span>
              </div>
              <button>✕</button>
            </label>
          </li>
          <li>
            <label
              ><input type="radio" name="category" />
              <div>
                <i class="fas fa-piggy-bank"></i>
                <span>적금</span>
              </div>
              <button>✕</button>
            </label>
          </li>
        </ul>

        <button>수정</button>
      </form>
      <!-- <button>삭제</button> -->
    </div>

    <div class="category-edit-cont">
      <strong>카테고리 추가</strong>
      <b class="explanation"
        >* 추가/수정 할 카테고리명 입력 후 원하는 아이콘을 선택해 주세요</b
      >
      <form action="">
        <input type="text" placeholder="추가할 카테고리를 입력해 주세요" />

        <ul>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-wallet"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-piggy-bank"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-shopping-cart"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-shopping-basket"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-gifts"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-birthday-cake"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-tshirt"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-baby"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-child"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-bicycle"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-basketball-ball"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-futbol"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-bone"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-cat"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-briefcase-medical"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-clinic-medical"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-bus"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-car"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-subway"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-charging-station"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-gas-pump"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-home"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-building"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-school"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-utensils"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-hamburger"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-pizza-slice"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-cocktail"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-coffee"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-beer"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-suitcase-rolling"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-plane"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-couch"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-camera"></i>
            </label>
          </li>
          <li>
            <label for="">
              <input type="radio" name="icon" />
              <i class="fas fa-desktop"></i>
            </label>
          </li>
        </ul>

        <!-- 위의 수정 버튼을 누르면 '추가'버튼이 '수정'으로 바뀌도록 할 것 -->
        <button>추가</button>
        <!-- <button>수정</button> -->
      </form>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
