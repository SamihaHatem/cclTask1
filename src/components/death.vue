<script>

export default {
  data() {

    return {
      fullName: ''
    }
  }
}

</script>

<template>
<div class="container">
<h3 class="text-blue">شهادة الميلاد</h3>


<form>


<div class="mb-3">
  <label for="fullName" class="form-label">الاسم رباعى لصاحب الشهادة</label>
  <input v-model="fullName" type="text" class="form-control" id="fullName">
</div>
{{fullName}}
<div class="mb-3">
  <label for="motherFullName" class="form-label">الاسم رباعى للأم</label>
  <input type="text" class="form-control" id="motherFullName">
</div>


<div class="mb-3">
<label class="form-label">النوع</label>
<select class="form-select" aria-label="Gender">
  <option value="M">ذكر</option>
  <option value="F">انثى</option>
</select>
</div>


<div class="mb-3">
  <label for="nationalIdenNumber" class="form-label">الرقم القومى</label>
  <input type="number" class="form-control" id="nationalIdenNumber" minLength=14 maxLegth=14>
</div>

<div class="mb-3">
<label class="form-label">صله القرابة</label>
<select class="form-select" aria-label="relationCode">
  <option value="default" class="text-secondary" selected disabled>اختر صله القرابة</option>
  <option value="FATHER">الأب</option>
  <option value="MATHER">الأم</option>
</select>
</div>

<div class="mb-3">
  <label for="numberOfCopies" class="form-label"> عدد النسخ</label>
  <input type="number" class="form-control" id="numberOfCopies">
</div>

<div class="mb-3">
  <label for="numberOfCopies" class="form-label"> عدد النسخ</label>
  <input type="number" class="form-control" id="numberOfCopies">
</div>

<button type="submit" class="btn btn-primary"> ارسال طلب </button>
</form>

 </div>
</template>

<style >
.text-blue{
    color:blue;
}

.m-auto-10{
    margin: auto 10px;
}
</style>
