<template>
  <div class="bg-pattern-top"></div>
  <div class="bg-pattern-bottom"></div>
  <main>
    <div class="card">
      <div class="card-banner">
        <img
          class="img-avatar"
          src="../src/assets/image-victor.jpg"
          alt="user profile pic"
        />
      </div>

      <div class="user-info">
        <h1 class="user-name">Victor Crest <span class="user-age">26</span></h1>
        <h2 class="user-location">London</h2>
      </div>
      <div class="stats">
        <ul class="user-stats">
          <li class="stats-followers">
            <ul>
              <li class="stats-count">80K</li>
              <li class="stats-label">Followers</li>
            </ul>
          </li>
          <li class="stats-likes">
            <ul>
              <li class="stats-count">803K</li>
              <li class="stats-label">Likes</li>
            </ul>
          </li>
          <li class="stats-photos">
            <ul>
              <li class="stats-count">1.4K</li>
              <li class="stats-label">Photos</li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<style scoped>
main {
  display: -ms-grid;
  display: grid;
  place-content: center;
  min-height: 100vh;
}

.card {
  text-align: center;
  -webkit-box-shadow: 3px 3px 15px hsla(0, 0%, 0%, 0.218);
  box-shadow: 3px 3px 15px hsla(0, 0%, 0%, 0.218);
  border-radius: 1em;
  min-width: 320px;
}

.card-banner {
  background-color: hsl(0deg 0% 23.94%);
  background-image: url(./assets/pattern.svg);
  background-size: 18% auto;
  background-position: center top;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  width: 100%;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  border-radius: 1em 1em 0 0;
  z-index: 999;
}

.user-info {
  background-color: var(--dark-blue);
  padding: 4.5rem 0 1rem 0;
  border-bottom: 1px solid hsla(0, 0%, 71%, 0.267);
}

.img-avatar {
  border-radius: 100px;
  border: 5px solid var(--dark-blue);
  position: relative;
  top: 3rem;
  z-index: 9999;
  height: 110px;
  width: 110px;
}

.img-avatar:hover {
  border-color: var(--blue);
  cursor: pointer;
  -webkit-transition: all 0.2s ease;
  -o-transition: all 0.2s ease;
  transition: all 0.2s ease;
}

.user-name {
  font-size: 1.2rem;
  color: var(--desaturated-blue);
}

.user-age {
  font-weight: 400;
  color: var(--dark-gray);
}

.user-location {
  color: var(--dark-gray);
  font-size: 0.95rem;
  font-weight: 400;
}

.user-stats {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: space-evenly;
  -ms-flex-pack: space-evenly;
  justify-content: space-evenly;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  background-color: var(--dark-blue);
  padding: 1.15rem;
  border-radius: 0 0 1em 1em;
}

.stats-count {
  font-size: 1.15rem;
  font-weight: 700;
  color: var(--desaturated-blue);
}

.stats-label {
  font-size: 0.65rem;
  color: var(--dark-gray);
  letter-spacing: 1px;
}

@media (width>=64rem) {
  .card {
    width: 21.75rem;
  }

  .card-banner {
    height: 8.75rem;
  }

  .img-avatar {
    top: 5rem;
  }

  .user-stats {
    padding: 1.5rem;
  }
}
</style>
