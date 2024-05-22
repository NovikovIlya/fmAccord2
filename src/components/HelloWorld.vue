<script setup lang="ts">

</script>

<template>
  <main>
    <div class="header">
      <img src="../assets/images/icon-star.svg"/>
      <h1>FAQs</h1>
    </div>
    <details>
      <summary class="sum">
        <span class="text">What is Frontend Mentor, and how will it help me?</span>
        <img id="image" src="../assets/images/icon-plus.svg" alt="" />
      </summary>
      <p>Frontend Mentor offers realistic coding challenges to help developers improve their frontend coding skills with projects in HTML, CSS, and JavaScript. It's suitable for all levels and ideal for portfolio building</p>
    </details>

    <details>
      <summary class="sum">
        <span class="text">Is Frontend Mentor free?</span>
        <img id="image" src="../assets/images/icon-plus.svg" alt="" />
      </summary>
      <p>Yes, Frontend Mentor offers both free and premium coding challenges, with the free option providing access to a range of projects suitable for all skill levels</p>
    </details>

    <details>
      <summary class="sum">
        <span class="text">Can I use Frontend Mentor projects in my portfolio?</span>
        <img id="image" src="../assets/images/icon-plus.svg" alt="" />
      </summary>
      <p>Yes, you can use projects completed on Frontend Mentor in your portfolio. It's an excellent way to showcase your skills to potential employers</p>
    </details>

    <details>
      <summary class="sum">
        <span class="text">How can I get help if I'm stuck on a Frontend Mentor challenge?</span>
        <img id="image" src="../assets/images/icon-plus.svg" alt="" />
      </summary>
      <p>The best place to get help is inside Frontend Mentor's Discord community. There's a help channel where you can ask questions and seek support from other community members.
</p>
    </details>

  </main>
</template>

<style scoped>
main{
  margin-top: 20%;
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  height: fit-content;
  width: 50%;
}
details > summary {
  list-style: none;
}
details > summary::-webkit-details-marker {
  display: none;
}
details::after{
  content:'';
  border:1px solid rgba(0, 0, 0, 0.051);
  display: flex;

  margin-bottom: 10px;
}
details:last-child::after {
  border: none;
  margin-top: 0px;
  margin-bottom:0px;
}
.header{
  display: flex;
  margin-bottom: 10px;
  gap:10px;
}
p{
  margin-bottom: 10px;
}
details[open] summary img {
  transition: all 1.5s ease-in-out;
  transform: rotate(180deg);
  /* Изображение при открытии details */
  content: url("../assets/images/icon-minus.svg");
}
.text{
  font-weight: bold;
}
.sum{
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap:20px;
  margin-bottom: 10px;
}

details summary img {
  transition: all 1.5s ease-in-out;
}
details summary img:hover {
  cursor:pointer;
}

@media screen and (max-width: 768px) {
  main{
    width: 90%;
  }
}


</style>
