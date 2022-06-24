<template>
  <div>
    <div class="container">
      <div class="practice">
        <p class="practice-text">Amaliyot kuni:</p>
        <span class="practice-time">14.09.2021</span>
        <input
          class="search-project"
          type="text"
          name="search"
          aria-label="search-project"
          placeholder="Qanday loyihani qidiramiz?"
        />
      </div>

      <div class="project">
        <ul class="project-list">
          <li class="project-item">
            <div class="project-inner">
              <button class="project-inner__btn">
                <img
                  src="../../assets/info-btn-background.svg"
                  alt="info-project"
                  width="17"
                  height="17"
                />
              </button>
              <p class="project-inner__info">
                Ushbu dastur Savdo markazlaridagi xodimlarning mijozlar bilan
                savdo qilish ya’ni ko‘rsatgan xizmatini baholash uchun
                mo’ljallangan dastur hisoblanadi!
              </p>
              <img
                class="project-inner__img"
                src="../../assets/project-crm-image.png"
                alt="project-image"
                width="34"
                height="34"
              />
              <span class="project-inner__span">Loyiha nomi</span>
              <h4 class="project-inner__heading">“Main CRM” dasturi</h4>
              <a class="project-inner__link" href="#">Dasturga kirish</a>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>

<style>
/* Header styles */
.container {
  padding-left: 40px;
  padding-right: 40px;
}

.practice {
  display: flex;
  align-items: center;
  padding-top: 15px;
  padding-bottom: 15px;
}

.practice-text {
  width: 110px;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 16px;
  letter-spacing: -0.01em;
  color: #000000;
  margin: 0;
  margin-right: 14px;
}

.practice-time {
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 16px;
  letter-spacing: -0.01em;
  color: #000000;
  display: flex;
  align-content: center;
}

.practice-time::before {
  content: "";
  width: 20px;
  height: 20px;
  background-image: url(../../assets/practice-time-calendar.svg);
  background-repeat: no-repeat;
  background-position: center;
  margin-right: 7px;
  margin-top: -3px;
}

.search-project {
  width: 440px;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 17px;
  color: #a3a3a3;
  margin-left: 61px;
  border: none;
  padding: 11px 11px 11px 14px;
  background-image: url(../../assets/search-icon.svg);
  background-repeat: no-repeat;
  background-position: calc(215px - -215px) 10px;
  background-size: auto;
}

/* Projects list styles */

.project {
  margin-top: 40px;
}

.project-list {
  margin: 0;
  list-style-type: none;
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.project-item {
  max-width: 312px;
  padding: 16px 16px 32px 16px;
  background-color: #ffffff;
  box-shadow: 0px 4px 20px rgba(181, 181, 181, 0.08);
  border-radius: 4px;
  margin-bottom: 20px;
}

.project-item:not(:last-child) {
  margin-right: 20px;
}

.project-inner__btn {
  border: none;
  margin-left: auto;
  margin-bottom: 29px;
  cursor: pointer;
}

.project-inner {
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.project-inner__info {
  display: none;
  position: absolute;
  width: 266px;
  background-color: #fff;
  box-shadow: 0px 6px 14px rgba(128, 128, 128, 0.05);
  border-radius: 4px;
  right: -13px;
  top: 20px;
}

.project-inner__img {
  margin-bottom: 50px;
}

.project-inner__span {
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 19px;
  color: #7b7b7b;
}

.project-inner__heading {
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  line-height: 140%;
  text-align: center;
  letter-spacing: -0.01em;
  margin: 0;
  margin-bottom: 48px;
}

.project-inner__link {
  width: 280px;
  font-style: normal;
  font-weight: 700;
  font-size: 16px;
  line-height: 140%;
  text-align: center;
  text-transform: uppercase;
  text-decoration: none;
  color: #5ec329;
  border: 1.5px solid #5ec329;
  border-radius: 2px;
  padding: 12px;
  transition: background-color 0.4s ease, color 0.4s ease;
}

.project-inner__link:hover {
  background-color: #5ec329;
  color: #ffffff;
}
</style>
