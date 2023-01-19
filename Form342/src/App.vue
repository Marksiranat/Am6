<script>
export default {
  data() {
    return {
      picked: "One",
    };
  },
};
</script>

<template>
  <div class="container m-1">
    <div>
      <img style="height: 150px; width: 150" src="./assets/MJU_LOGO.svg.png" alt="" />
    </div>
  </div>
  <div class="container">
    <div class="row text-center">
      <h3>คําร้องขอลงทะเบียนเรียนเพื่อให้ได้ค่าระดับคะแนนเป็น S หรือ U</h3>
    </div><br>
    <div class="row d-flex justify-content-center">
      <div><input type="date" /></div>
      <div>
        เรื่อง ขอลงทะเบียนเรียนเพื่อให้ได้ค่าระดับคะแนนเป็น Sหรือ U ภาคเรียนที่
        <input type="text" /> ปีการศึกษา<input type="text" />
      </div>
      <div>เรียน อาจารย์ผู้สอนวิชา <input type="text" /></div>
      <div>
        ข้าพเจ้า
        <input type="radio" id="one" value="นาย" v-model="picked" />
        <label for="นาย">นาย</label>
        <input type="radio" id="two" value="นาง" v-model="picked" />
        <label for="นาง">นาง</label>
        <input type="radio" id="two" value="นางสาว" v-model="picked" />
        <label for="นางสาว">นางสาว</label>
        ชื่อ-นามสกุล <input type="text" />
      </div>
      <br />
      <div>
        รหัสนักศึกษา (10หลัก) <input type="number" /> โทรศัพท์มือถือ (10หลัก)
        <input type="tel" />
      </div>
      <br />
      <div>
        หลักสูตร ปริญญาตรี
        <input type="radio" id="one" value="4-5ปี" v-model="picked" />
        <label for="4-5ปี">4-5ปี</label>
        <input type="radio" id="one" value=" 4ปีเทียบเข้าเรียน(2ปี) " v-model="picked" />
        <label for=" 4ปีเทียบเข้าเรียน(2ปี) "> 4 ปีเทียบเข้าเรียน (2ปี) </label>
        <input type="radio" id="one" value=" บัณฑิตศึกษา " v-model="picked" />
        <label for=" บัณฑิตศึกษา "> บัณฑิตศึกษา </label>
        <input type="radio" id="one" value=" ภาคปกติ " v-model="picked" />
        <label for=" ภาคปกติ "> ภาคปกติ </label>
        <input type="radio" id="one" value=" ภาคสมทบ" v-model="picked" />
        <label for=" ภาคสมทบ "> ภาคสมทบ </label>
      </div>
      <br />

      <div>
        สาขา
        <select name="" id="" v-model="Transfer_to">
          <option value="เกษตรศาสตร์">เกษตรศาสตร์</option>
          <option value="พืชสวน">พืชสวน</option>
          <option value="เทคโนโลยีอาหาร">เทคโนโลยีอาหาร</option>
          <option value="เทคโนโลยีอุสาหการ การผลิต">เทคโนโลยีอุสาหการ การผลิต</option>
          <option value="เทคโนโลยีพอลิเมอร์">เทคโนโลยีพอลิเมอร์</option>
          <option value="วิศวกรรมเกษตร">วิศวกรรมเกษตร</option>
          <option value="วิศวกรรมอาหาร">วิศวกรรมอาหาร</option>
          <option value="คณิตศาสตร์">คณิตศาสตร์</option>
          <option value="เคมี">เคมี</option>
          <option value="เทคโนโลยีชีวภาพ">เทคโนโลยีชีวภาพ</option>
          <option value="ฟิสิกส์">ฟิสิกส์</option>
          <option value="วัสดุศาสตรฺ">วัสดุศาสตรฺ</option>
          <option value="สถิติ">สถิติ</option>
          <option value="เทคโนโลยีสารสนเทศ">เทคโนโลยีสารสนเทศ</option>
          <option value="วิทยาการคอมพิวเตอร์">วิทยาการคอมพิวเตอร์</option>
          <option value="รัฐประศาสนศาสตร์">รัฐประศาสนศาสตร์</option>
          <option value="รัฐศาสตร์">รัฐศาสตร์</option>
          <option value="การเงิน">การเงิน</option>
          <option value="การจัดการ">การจัดการ</option>
          <option value="การบัญชี">การบัญชี</option>
          <option value="การตลาด">การตลาด</option>
          <option value="ระบบสารสนเทศ">ระบบสารสนเทศ</option>
          <option value="การท่องเที่ยวและการโรงแรม">การท่องเที่ยว และ การโรงแรม</option>
          <option value="ประมง">ประมง</option>
          <option value="เศรษฐศาสตร์">เศรษฐศาสตร์</option>
          <option value="นิเทศศาสตร์">นิเทศศาสตร์</option>
          <option value="อังกฤษ">อังกฤษ</option>
          <option value="วิศวกรรมพลังงาน">วิศวกรรมพลังงาน</option>
          <option value="ดิจิทัล">ดิจิทัล</option>
          <option value="ภูมิสถาปัตยกรรม">ภูมิสถาปัตยกรรม</option>
          <option value="วางแผนภาคและเมือง">วางแผนภาคและเมือง</option>
          <option value="สถาปัตยกรรม">สถาปัตยกรรม</option>
          <option value="สัตวศาสตร์">สัตวศาสตร์</option>
          <option value="วนศาสตร์">วนศาสตร์</option>
          <option value="สังคมศาสตร์และพฤติกรรมศาสตร์">
            สังคมศาสตร์และพฤติกรรมศาสตร์
          </option>
          <option value="การปกครอง">การปกครอง</option>
        </select>
        คณะ
        <select name="" v-model="Group">
          <option value="คณะผลิตกรรมการเกษตร">คณะผลิตกรรมการเกษตร</option>
          <option value="คณะบริหารธุรกิจ">คณะบริหารธุรกิจ</option>
          <option value="คณะวิทยาศาสตร์">คณะวิทยาศาสตร์</option>
          <option value="คณะศิลปศาสตร์">คณะศิลปศาสตร์</option>
          <option value="คณะสถาปัตยกรรมศาสตร์ และการออกแบบสิ่งแวดล้อม ">
            คณะสถาปัตยกรรมศาสตร์ และการออกแบบสิ่งแวดล้อม
          </option>
          <option value="คณะเทคโนโลยีการประมง และทรัพยากรทางน้ำ">
            คณะเทคโนโลยีการประมง และทรัพยากรทางน้ำ
          </option>
          <option value="คณะวิศวกรรมและอุตสาหกรรมเกษตร ">
            คณะวิศวกรรมและอุตสาหกรรมเกษตร
          </option>
          <option value="คณะพัฒนาการท่องเที่ยว ">คณะพัฒนาการท่องเที่ยว</option>
          <option value="คณะเศรษฐศาสตร์ ">คณะเศรษฐศาสตร์</option>
          <option value="วิทยาลัยบริหารศาสตร์ ">วิทยาลัยบริหารศาสตร์</option>
          <option value="วิทยาลัยพลังงานทดแทน ">วิทยาลัยพลังงานทดแทน</option>
          <option value="วิทยาลัยนานาชาติ ">วิทยาลัยนานาชาติ</option>
          <option value="มหาวิทยาลัยแม่โจ้-แพร่ เฉลิมพระเกียรติ ">
            มหาวิทยาลัยแม่โจ้-แพร่ เฉลิมพระเกียรติ
          </option>
          <option value="มหาวิทยาลัยแม่โจ้-ชุมพร ">มหาวิทยาลัยแม่โจ้-ชุมพร</option>
          <option value="คณะพยาบาลศาสตร์">คณะพยาบาลศาสตร์</option>
          <option value="คณะสัตวแพทย์ศาสตร์">คณะสัตวแพทย์ศาสตร์</option></select>
          <br>
        <div>
          มีความประสงค์จะขออนุญาตลงทะเบียนเรียนวิชา <input type="text" />จํานวน
          <input type="number" />หน่วยกิตซึ่งการลงทะเบียนเรียนครั้งนี้
          โดยไม่มีแต้มระดับคะแนนและถ้ามีผลการศึกษาเป็นที่พอใจจะได้ระดับคะแนนเป็น S
          (Satisfactory) หรือไม่เป็นที่พอใจ จะได้ระดับคะแนนเป็น U (Unsatisfactory)
          จึงเรียนมาเพื่อโปรดพิจารณา
        </div>
      </div>
    </div>
  </div>
</template>

<style></style>
