<template>
  <main class="">
    <section class="contain body">
      <div class="contained">
        <div class="top">
          <h1>Join our community</h1>
          <h2>30-day, hassle-free money back guarantee</h2>
          <p>
            Gain access to our full library of tutorials along with expert code
            reviews. Perfect for any developers who are serious about honing
            their skills.
          </p>
        </div>
        <div class="bottom">
          <div>
            <h1>Monthly Subscription</h1>
            <div>
              <h2>$29</h2>
              <span>per month</span>
            </div>
            <p>Full access for less than $1 a day</p>
            <button>Sign Up</button>
          </div>
          <div>
            <h1>Why Us</h1>
            <ul>
              <li>Tutorials by industry experts</li>
              <li>Peer &amp; expert code review</li>
              <li>Coding exercises</li>
              <li>Access to our GitHub repos</li>
              <li>Community forum</li>
              <li>Flashcard decks</li>
              <li>New videos every week</li>
            </ul>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>



<style>
@import url("https://fonts.googleapis.com/css2?family=Karla:wght@400;700&display=swap");

:root {
  --small-font-weight: 400;
  --big-font-weight: 700;
  --minor-color: hsl(218, 22%, 67%);
  --major-color: hsl(71, 73%, 54%);
  --main-background: hsl(204, 43%, 93%);
  --minor-background: hsl(179, 62%, 43%);
}
.body {
  font-family: "Karla", sans-serif;
  font-size: 16px !important;
  background-color: var(--main-background);
}
ul {
  list-style: none;
  padding: 0;
}
.contain {
  display: grid;
  place-items: center;
  height: 100vh;
  padding: 0 1rem;
}
.contained {
  max-width: 768px;
  width: 100%;
  border-radius: 10px;
  overflow: hidden;
}
.top {
  background-color: white;
  padding: 2.5rem;
}

.top h1 {
  color: var(--minor-background);
  font-weight: var(--big-font-weight);
  /* font-size: 18px; */
}

.top h2 {
  font-weight: var(--big-font-weight);
  margin: 1.5rem 0;
  font-size: 20px;
  color: var(--major-color);
}
.top p {
  font-weight: var(--big-font-weight);
  color: var(--minor-color);
}

.bottom {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}

.bottom div:first-child {
  background-color: var(--minor-background);
  padding: 2.5rem;
}

.bottom h1 {
  color: white;
  font-size: 20px;
  font-weight: var(--big-font-weight);
}
.bottom div:first-child div {
  background-color: var(--minor-background);
  padding: 1rem 0;
  display: flex;
  align-items: center;
  gap: 0.7rem;
}
.bottom div:first-child div h2 {
  color: white;
  font-size: 30px;
  font-weight: var(--big-font-weight);
}
.bottom div:first-child div span {
  color: rgba(255, 255, 255, 0.575);
  /* font-size: 30px; */
  font-weight: var(--big-font-weight);
}
.bottom div:first-child p {
  color: rgba(255, 255, 255, 0.767);
  /* font-size: 30px; */
  font-weight: var(--big-font-weight);
}
.bottom div:first-child button {
  outline: none;
  border: 0;
  margin: 1rem 0 0 0;
  border-radius: 5px;
  font-size: 16px;
  color: white;
  box-shadow: 0px 3px 19px 1px rgba(39, 39, 39, 0.384);
  padding: 1.3rem;
  background-color: var(--major-color);
  width: 100%;
  font-weight: var(--big-font-weight);
  cursor: pointer;
}

.bottom div:last-child {
  background-color: hsl(179, 70%, 45%);
  padding: 2.5rem;
}

.bottom div:last-child ul {
  padding: 1rem 0 0 0;
  color: rgba(255, 255, 255, 0.767);
  /* font-size: 30px; */
  font-weight: var(--big-font-weight);
}

.bottom div:last-child ul li {
  padding: 0 0 0.21rem 0;
}

@media screen and (max-width: 768px) {
  .bottom {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
  }
  .bottom div:first-child,
  .top,
  .bottom div:last-child {
    padding: 1.5rem;
  }
  .top h1 {
    font-size: 20px;
  }

  .top h2 {
    font-size: 18px;
  }
  .top p {
    line-height: 1.5rem;
    font-size: 14px;
  }
}
</style>