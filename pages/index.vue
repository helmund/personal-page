<template>
  <div>
    <div class="container">
      <div class="intro">
        <div class="intro__kicker">
          Hey<i class="wave">👋</i>, ich bin
        </div>
        <h1 class="intro__headline">
          <span class="intro__name">Sascha Helmund</span>
          <small class="intro__desc">
            <i>👨🏻‍💻</i>Frontend-Entwickler aus <i>📍</i>Leipzig
          </small>
        </h1>
      </div>
    </div>
    <div class="container">
      <div class="resume">
        <h2>Berufserfahrung</h2>
        <ul class="resume__list">
          <li class="resume__list-item">
            <article class="resume-item">
              <h3 class="resume-item__company">
                Mogic GmbH
              </h3>
              2017 - heute
              Teamleiter Frontend Entwicklung
            </article>
          </li>
          <li class="resume__list-item">
            <article class="resume-item">
              <h3 class="resume-item__company">
                Mogic GmbH
              </h3>
              2012 - heute
              Frontend-Entwickler
            </article>
          </li>
          <li class="resume__list-item">
            <article class="resume-item">
              <h3 class="resume-item__company">
                Druck und Werte GmbH
              </h3>
              2011
              Trainee Web-Entwicklung
            </article>
          </li>
          <li class="resume__list-item">
            <article class="resume-item">
              <h3 class="resume-item__company">
                Dirk Rossmann GmbH
              </h3>
              2008 - 2010
              Merchandiser
            </article>
          </li>
          <li class="resume__list-item">
            <article class="resume-item">
              <h3 class="resume-item__company">
                SCS GMBH
              </h3>
              2004 - 2007
              Ausbildung Mediengestalter
            </article>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
html {
  font-family: 'Inconsolata', monospace;
  background-color: #212121;
  color: #bdbdbd;
  padding: 10px;
}
</style>

<style lang="scss" scoped>

.intro {
  &__headline {
    display: block;
    font-family: 'Playfair Display', serif;
    font-size: clamp(1rem, 6vw + 1rem, 10rem);
    line-height: 0.85;
    letter-spacing: 0.5px;
    text-transform: uppercase;
  }
  &__desc {
    margin: 0.25em 0;
    display: block;
    font-size: 0.5em;
    text-transform: none;
    line-height: 1;
  }

  &__name {
    // white-space: nowrap;
    // line-height: 0.85;
  }

  &__kicker {
    font-size: 2rem;
    font-size: clamp(1rem, 2vw + 1rem, 3rem);
  }
}

i {
  display: inline-block;
  font-size: 0.85em;
  font-style: normal;
}

.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: left;
}

.resume {
  &__list {
    margin: 0;
    padding: 0;
    list-style-type: none;
  }

  &__list-item {
    padding: 10px 0;
  }
}

.wave {
  animation-name: wave-animation;
  animation-duration: 2.5s;
  animation-iteration-count: infinite;
  transform-origin: 70% 70%;
}

@keyframes wave-animation {
    0% { transform: rotate( 0.0deg) }
   10% { transform: rotate(14.0deg) }
   20% { transform: rotate(-8.0deg) }
   30% { transform: rotate(14.0deg) }
   40% { transform: rotate(-4.0deg) }
   50% { transform: rotate(10.0deg) }
   60% { transform: rotate( 0.0deg) }
  100% { transform: rotate( 0.0deg) }
}

</style>
