<script setup>
import { ref } from "vue";
const stuID = ref("");
const stuNAME = ref("");
</script>

<template>
  <div class="d-flex justify-content-center">
    <img
      style="height: 170px"
      src="https://upload.wikimedia.org/wikipedia/th/thumb/b/b7/MJU_LOGO.svg/1200px-MJU_LOGO.svg.png"
    />
    <h1 class="align-self-center">คำร้องขอทั่วไป</h1>
  </div>

  <form>
    <div class="d-flex justify-content-end my-3">
      วันที่<br />
      <input type="date" name="" id="" required />
    </div>

    <div class="my-3">เรื่อง <input type="text" name="" id="" required /></div>

    <div class="my-3">เรียน <input type="text" name="" id="" required /></div>

    <div class="my-3">
      ข้าพเจ้า
      <div class="form-check form-check-inline">
        <input
          class="form-check-input"
          type="radio"
          name="flexRadioDefault"
          id="flexRadioDefault1"
        />
        <label class="form-check-label" for="flexRadioDefault1"> นาย </label>
      </div>
      <div class="form-check form-check-inline">
        <input
          class="form-check-input"
          type="radio"
          name="flexRadioDefault"
          id="flexRadioDefault2"
          checked
        />
        <label class="form-check-label" for="flexRadioDefault2"> นาง </label>
      </div>
      <div class="form-check form-check-inline">
        <input
          class="form-check-input"
          type="radio"
          name="flexRadioDefault"
          id="flexRadioDefault3"
        />
        <label class="form-check-label" for="flexRadioDefault3"> นางสาว </label>
      </div>
      ชื่อ
      <input type="text" name="stuNAME" id="" maxlength="30" required />
      สกุล
      <input type="text" name="" id="" maxlength="30" required />
      รหัสนักศึกษา
      <input
        type="text"
        v-model="stuID"
        name="stuID"
        id=""
        maxlength="10"
        required
      /><br />
    </div>

    สาขาวิชา <input type="text" name="" id="" />
    คณะ
    <select name="" id="">
      <option style="text-align: center">---- กรุณาเลือกคณะ ----</option>
      <option>คณะวิทยาศาสตร์</option>
      <option>คณะบริหารธุรกิจ</option>
      <option>คณะเทคโนโลยีการประมงและทรัพยากรทางน้ำ</option>
      <option>คณะศิลปศาสตร์</option>
      <option>คณะสถาปัตยกรรมศาสตร์ และการออกแบบสิ่งแวดล้อม</option>
      <option>คณะสารสนเทศและการสื่อสาร</option>
      <option>คณะผลิตกรรมการเกษตร</option>
      <option>คณะวิศวกรรมและอุตสาหกรรมเกษตร</option>
      <option>คณะพัฒนาการท่องเที่ยว</option>
      <option>คณะเศรษฐศาสตร์</option>
      <option>คณะสัตวศาสตร์และเทคโนโลยี</option>
      <option>คณะสัตวแพทยศาสตร์</option>
      <option>คณะพยาบาลศาสตร์</option>
    </select>
    เบอร์โทร <input type="text" name="" id="" maxlength="10" required />
    <div>
      <hr />
      <label for="reason" class="form-label">ระบุเหตุผลประกอบคำร้อง</label>
      <textarea class="form-control" id="reason" rows="3" required></textarea>
    </div>
    <div>
      <hr />
      <div class="d-flex justify-content-center my-3">ลงชื่อนักศึกษา</div>
      <div class="d-flex justify-content-center">
        <input type="text" name="" id="" required maxlength="30" />
      </div>
    </div>
    <div class="d-flex justify-content-center my-3">
      <input
        type="submit"
        value="ส่งคำร้องขอ"
        onclick="alert('ส่งข้อมูลสำเร็จ!')"
      />
    </div>
  </form>
</template>

<style scoped></style>

<script></script>
