<script setup>
import { toast } from 'vue3-toastify';
import 'vue3-toastify/dist/index.css';

toast.info("ยินดีต้อนรับเข้าสู่ 7 ประเทศน่าอยู่", {
  autoClose: 1500,
  position:toast.POSITION.TOP_CENTER
})

const notify = () => {
  toast.success("ยินดีต้อนรับเข้าสู่ 7 ประเทศน่าอยู่", {
    autoClose: 1500,
    position: toast.POSITION.TOP_CENTER
  })
  return notify
}

</script>

<template>
  <div class="container my-5">
    <div class="card shadow" style="width: 20rem;">
      <div class="card-header p-0">
        <img src="https://www.kkday.com/th/blog/wp-content/uploads/Grindelwald-Switzerland.jpg" class="card-img-top"
          alt="img">
      </div>
      <div class="card-body">
        <h5 class="card-title">7 ประเทศ น่าอยู่ (7 countries worth living in)</h5>
        <p class="card-text">เป็นบริเวณที่ระบุเป็นหน่วยต่างหากในภูมิศาสตร์การเมือง ประเทศอาจเป็นรัฐเอกราชหรือรัฐที่ถูกรัฐอื่นยึดครอง เป็นรัฐซึ่งไร้เอกราชหรืออดีตเขตปกครองทางการเมืองเอกราช หรือพื้นที่ภูมิศาสตร์ซึ่งเป็นที่ตั้งของประชาชนที่เดิมไม่ขึ้นต่อกันหรือมีความสัมพันธ์ต่างกันซึ่งมีลักษณะทางการเมืองเป็นเอกลักษณ์.</p>
        <a href="#" class="btn btn-primary" @click="notify">Read...</a>
      </div>
    </div>
  </div>
</template>
