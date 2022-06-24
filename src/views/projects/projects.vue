<template>
  <div>
    <div class="main-wrapper">
      <div class="left-content">
        <ul class="info-list">
          <li class="info-list__item">
            <a class="info-list__link dashboard-link" href="#">Dashboard</a>
          </li>
          <li class="info-list__item active-item">
            <a
              class="info-list__link projects-link__active active-link"
              href="#"
              >Dasturlar</a
            >
          </li>
          <li class="info-list__item not-active--item">
            <a class="info-list__link users-link not-active--link" href="#"
              >Foydalanuvchilar</a
            >
          </li>
        </ul>

        <div class="wrapper">
          <button class="hide-panel__btn" type="button">
            Panelni yashirish
          </button>
          <p class="project-version__text">Dasturning hozirgi versiyasi:</p>
          <span class="project-version">Version 7.1.15</span>
        </div>
      </div>

      <div class="right-content">
        <div class="header">
          <div class="practice">
            <p class="practice-text">Amaliyot kuni:</p>
            <span class="practice-time">14.09.2021</span>
            <button class="practice-add__btn" type="button">
              <img src="../../assets/add-btn.svg" width="14" height="14" />
            </button>
            <input
              class="search-project"
              type="text"
              name="search"
              aria-label="search-project"
              placeholder="Qanday loyihani qidiramiz?"
            />
          </div>

          <div class="user">
            <div class="user-inner">
              <h4 class="user-name">Akbarjon Anvarjonov</h4>
              <p class="user-position">Dasturlash bo‘limi boshlig‘i</p>
            </div>
            <img
              class="user-notification"
              src="../../assets/notification-icon.svg"
              alt="icon-notification"
              width="20"
              height="21"
            />
            <div class="user-avatar">
              <button class="user-avatar__btn">
                <img
                  class="user-avatar__img"
                  src="../../assets/user-avatar.png"
                  alt="user-avatar"
                  width="42"
                  height="42"
                />
              </button>

              <div class="user-cabinet">
                <div class="user-cabinet__inner">
                  <div class="user-cabinet__div">
                    <img
                      class="user-cabinet__img"
                      src="../../assets/user-avatar.png"
                      alt="user-avatar"
                      width="40"
                      height="40"
                    />
                    <div class="user-cabinet__info">
                      <p class="user-cabinet__name">Akbarjon Anvarjonov</p>
                      <span class="user-cabinet__position"
                        >Dasturlash bo‘limi boshlig‘i</span
                      >
                    </div>
                  </div>
                  <div class="user-cabinet__links--wrapper">
                    <a class="user-cabinet__private" href="#"
                      >Shaxsiy kabinet</a
                    >
                    <a class="user-cabinet__exit" href="#">Chiqish</a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="projects-wrapper">
          <table class="projects-table" style="width: 100%">
            <tr>
              <th>ID</th>
              <th>Loyiha nomi</th>
              <th>Loyiha url</th>
              <th>Muhimlilik reytingi</th>
              <th>Aktivlashtirish</th>
              <th>Amallar</th>
            </tr>
            <tr>
              <td>1</td>
              <td><h4>“Main CRM” dasturi</h4></td>
              <td>192.168.11.20:4000</td>
              <td>1</td>
              <td>
                <label class="toggler-wrapper style">
                  <input type="checkbox" />
                  <div class="toggler-slider">
                    <div class="toggler-knob"></div>
                  </div>
                </label>
              </td>
              <td>
                <button class="edit-btn">
                  <svg
                    class="edit-btn__svg"
                    width="12"
                    height="12"
                    viewBox="0 0 12 12"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M6.6 2.57203L9.428 5.40069L2.828 12H0V9.17136L6.6 2.57136V2.57203ZM7.54267 1.62936L8.95667 0.214692C9.08169 0.0897111 9.25122 0.0195007 9.428 0.0195007C9.60478 0.0195007 9.77432 0.0897111 9.89933 0.214692L11.7853 2.10069C11.9103 2.22571 11.9805 2.39525 11.9805 2.57203C11.9805 2.7488 11.9103 2.91834 11.7853 3.04336L10.3707 4.45736L7.54267 1.62936Z"
                    />
                  </svg>
                </button>
              </td>
            </tr>
          </table>
        </div>
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
.main-wrapper {
  display: flex;
  align-items: flex-start;
  overflow: hidden;
}

.right-content {
  width: 100%;
  padding-right: 40px;
}

.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.user {
  display: flex;
  align-items: center;
}

.user-inner {
  margin-right: 22px;
}

.user-name {
  width: 160px;
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 19px;
  letter-spacing: -0.01em;
  color: #000000;
  margin: 0;
  margin-bottom: 2px;
}

.user-position {
  width: 140px;
  font-style: normal;
  font-weight: 500;
  font-size: 12px;
  line-height: 14px;
  letter-spacing: -0.01em;
  color: #a3a3a3;
  margin: 0;
}

.user-notification {
  margin-right: 22px;
  display: flex;
  align-items: center;
}

.user-notification::after {
  content: "";
  display: block;
  width: 12px;
  height: 12px;
  background-color: #ff4141;
  background-repeat: no-repeat;
  background-position: center;
  background-size: 12px;
  border: 1px solid #ffffff;
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

.practice-add__btn {
  background-color: #5ec329;
  box-shadow: 0px 2px 8px rgba(94, 195, 41, 0.25);
  border-radius: 8px;
  padding: 11px 13px;
  border: none;
  cursor: pointer;
  transition: opacity 0.4s ease;
  margin-left: 71px;
}

.practice-add__btn:hover {
  opacity: 0.7;
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

.user-cabinet {
  position: relative;
}

.user-cabinet__inner {
  display: none;
  width: 200px;
  position: absolute;
  right: 5px;
  top: -2px;
  padding: 20px 20px 24px 20px;
  background-color: #ffffff;
  box-shadow: 0px 10px 20px rgba(128, 128, 128, 0.08);
  border-radius: 4px;
  z-index: 1;
}

.user-avatar__btn {
  border: none;
  cursor: pointer;
}

.user-cabinet__div {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: flex-start;
}

.user-cabinet__info {
  width: 100%;
  text-align: left;
}

.user-cabinet__name {
  font-style: normal;
  font-weight: 600;
  font-size: 12px;
  line-height: 14px;
  color: #000000;
  margin: 0;
}

.user-cabinet__position {
  font-style: normal;
  font-weight: 400;
  font-size: 8px;
  line-height: 10px;
  color: #a4a6a4;
  margin: 0;
}

.user-cabinet__img {
  margin-right: 8px;
}

.user-cabinet__links--wrapper {
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  margin-top: 23px;
}

.user-cabinet__private {
  font-style: normal;
  font-weight: 500;
  font-size: 12px;
  line-height: 14px;
  color: #000000;
  text-decoration: none;
  display: flex;
  align-items: center;
  margin-bottom: 15px;
}

.user-cabinet__private::before {
  content: "";
  width: 13px;
  height: 17px;
  background-image: url(../../assets/user-icon-not-active.svg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  margin-right: 13px;
}

.user-cabinet__exit {
  font-style: normal;
  font-weight: 500;
  font-size: 12px;
  line-height: 14px;
  color: #000000;
  text-decoration: none;
  display: flex;
  align-items: center;
}

.user-cabinet__exit::before {
  content: "";
  width: 16px;
  height: 16px;
  background-image: url(../../assets/exit-icon.svg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  margin-right: 13px;
}

/* Left content */

.left-content {
  height: 100vh;
  padding: 73px 33px 30px 0;
}

.info-list {
  list-style: none;
  text-align: left;
  margin: 0;
  padding: 0;
}

.info-list__item {
  display: flex;
  align-items: center;
}

.info-list__item:not(:last-child) {
  margin-bottom: 20px;
}

.info-list__link {
  font-style: normal;
  font-weight: 700;
  font-size: 14px;
  line-height: 17px;
  letter-spacing: -0.04em;
  text-transform: uppercase;
  color: #000000;
  text-decoration: none;
  display: flex;
  align-items: center;
  transition: opacity 0.3s ease;
}

.info-list__link:hover {
  opacity: 0.7;
}

.dashboard-link {
  padding-left: 29px;
}

.dashboard-link::before {
  content: "";
  width: 21px;
  height: 21px;
  background-image: url(../../assets/dashboard-icon.svg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  margin-right: 12px;
  margin-bottom: 15px;
}

.active-link {
  color: #5ec329;
}

.projects-link::before {
  content: "";
  width: 21px;
  height: 21px;
  background-image: url(../../assets/projects-icon-not-active.svg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  margin-right: 12px;
}

.projects-link__active::before {
  content: "";
  width: 21px;
  height: 21px;
  background-image: url(../../assets/projects-icon-active.svg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  margin-right: 12px;
}

.users-link::before {
  content: "";
  width: 21px;
  height: 21px;
  background-image: url(../../assets/user-icon-not-active.svg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  margin-right: 12px;
}

.users-link__active::before {
  content: "";
  width: 21px;
  height: 21px;
  background-image: url(../../assets/user-icon-active.svg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  margin-right: 12px;
}

.active-item::before {
  content: "";
  width: 5px;
  height: 54px;
  background-image: url(../../assets/active-icon.svg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  margin-right: 22px;
}

.not-active--item::before {
  content: "";
  width: 5px;
  height: 54px;
  background-image: url(../../assets/hover.svg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  margin-right: 22px;
}

.wrapper {
  display: flex;
  flex-direction: column;
  padding-left: 30px;
}

.hide-panel__btn {
  font-style: normal;
  font-weight: 700;
  font-size: 11px;
  line-height: 13px;
  letter-spacing: -0.02em;
  text-transform: uppercase;
  color: #a3a3a3;
  border: none;
  cursor: pointer;
  display: flex;
  align-items: center;
  transition: opacity 0.3s ease;
}

.hide-panel__btn::before {
  content: "";
  width: 18px;
  height: 19px;
  background-image: url(../../assets/hide-panel-icon.svg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  margin-right: 7px;
}

.hide-panel__btn:hover {
  opacity: 0.7;
}

.project-version__text {
  font-style: normal;
  font-weight: 500;
  font-size: 12px;
  line-height: 14px;
  display: flex;
  align-items: center;
  color: #a3a3a3;
  margin: 0;
  margin-bottom: 5px;
  margin-top: 32px;
}

.project-version {
  font-style: normal;
  font-weight: 600;
  font-size: 12px;
  line-height: 14px;
  display: flex;
  align-items: center;
  color: #000000;
}

/* Projects table */
.projects-table {
  margin-top: 10px;
}

h4 {
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 18px;
  color: #000000;
  margin: 0;
}

th {
  font-style: normal;
  font-weight: 800;
  font-size: 13px;
  line-height: 16px;
  text-transform: uppercase;
  color: #000000;
}

tr {
  text-align: left;
}

td {
  text-align: left;
  padding-top: 20px;
}

.toggler-wrapper {
  display: block;
  width: 50px;
  height: 25px;
  cursor: pointer;
  position: relative;
}

.toggler-wrapper input[type="checkbox"] {
  display: none;
}

.toggler-wrapper input[type="checkbox"]:checked + .toggler-slider {
  background-color: #44cc66;
}

.toggler-wrapper .toggler-slider {
  background-color: #ccc;
  position: absolute;
  border-radius: 100px;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  transition: all 300ms ease;
}

.toggler-wrapper .toggler-knob {
  position: absolute;
  transition: all 300ms ease;
}

.toggler-wrapper.style
  input[type="checkbox"]:checked
  + .toggler-slider
  .toggler-knob {
  left: calc(100% - 19px - 3px);
}

.toggler-wrapper.style .toggler-knob {
  width: calc(25px - 6px);
  height: calc(25px - 6px);
  border-radius: 50%;
  left: 3px;
  top: 3px;
  background-color: #fff;
}

.edit-btn {
  fill: #fbc60d;
  width: 36px;
  height: 36px;
  border-radius: 50%;
  border: none;
  cursor: pointer;
  transition: background-color 0.3s ease, fill 0.3s ease;
}

.edit-btn:hover {
  background-color: #fbc60d;
  fill: #ffffff;
}
</style>
