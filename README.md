# journal-3

# Jan 24,2022 Felx page layout

TODO:

- create Navigation bar and style it

- put some Logos with Navigation

- put colors on navar

## The lesson we did

For today lesson we are talk about flex container and play with the flex container with codepen, you can see the pove of work.

### problem and solving:

I had issues about codepen CSS issues, the codepen showed me all css working and colors adding to it. How I did solved is I asked Ashyln about issues and she told me maybe codepen has issues so tried to start on other pages from codepen. 

### Code html: 

```
<div id="app">
  <header class="top-bar">
    <div class="logo-wrapper">
      <a href="#">
        <img src="https://img.icons8.com/color/30/000000/amazon-alexa-logo.png"/>
        <p>Awesome</p>
      </a>
    </div>
    <nav class="nav-wrapper">
      <ul class="nav-links">
        <li>
          <a href="#">Galatic Empire</a>
        </li>
        <li>
          <a href="#">Dark Side</a>
        </li>
        <li>
          <a href="#">About Us</a>
        </li>
      </ul>
    </nav>
    <div class="signup">
      <a href="#">
  <i class="las la-user-plus"></i>
      </a>
    </div>
  </header>
  <!-- site content -->
  <main>
    <header class="main-header">
      <h1>Your Galactic Empire</h1>
    </header>
    <section class="card-container">
      <article class="card">
        <div>
          <h3>Free</h3>
          <div class="card-img-wrapper">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQrumSUiaxb304miu9HGASw4_DUlmMWv4ul9w&usqp=CAU" />
          </div>
          <p>free</p>
        </div>
        <div>
          <p>gongyoo</p>
          <p>famouse actor</p>
        </div>
        <div>
          <a href="#" class="btn">Click here</a>
        </div>
      </article>
      <article class="card">
        <div>
          <h3>Free</h3>
          <div class="card-img-wrapper">
            <img src="https://assets.codepen.io/5580368/delesign-start-up.png" />
          </div>
          <p>Free Forever</p>
        </div>
        <div>
          <p>Up to 1GB</p>
          <p>Lorem ipsum dolor sit amet.</p>
        </div>
        <div>
          <a href="#" class="btn">Buy Now</a>
        </div>
      </article>
      <article class="card">
        <h3>Free</h3>
        <div class="card-img-wrapper">
          <img src="https://assets.codepen.io/5580368/delesign-start-up.png" />
        </div>
        <p>Free Forever</p>
        <p>Up to 1GB</p>
        <p>Lorem ipsum dolor sit amet.</p>
        <a href="#" class="btn">Buy Now</a>
      </article>
    </section>
  </main>
  <footer>
    <p>&copy; Darth Maul</p>
  </footer>
</div>
```



### css code:

```
/* *********** *
/* Base Styles */
/* *********** */
:root {
  --black: #010201;
  --light-red: #be4059;
  --red: #79102c;
  --white: #a8bcbd;
  --blue: #478ec3;
}
#app {
  display: flex;
  flex-direction: column;
}

.top-bar a {
  /* remove link color and underline */
  color: var(--white);
  text-decoration: none;
  display: block;
}
ul {
  /* remove list styles */
  list-style-type: none;
  padding: 0;
}
img {
  width: 100%;
  height: auto;
}
footer {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 5rem;
  margin-top: 10px;
  background-color: var(--black);
  color: var(--light-red);
}
/* *************** */
/* *** layout  *** */
/* *************** */

.top-bar {
  display: flex;
  justify-content: space-around;
  align-items: center;
  gap: 1rem;
  background-color: var(--black);
  color: var(--white);
  padding: 0 1rem;
}

.nav-wrapper {
  flex-grow: 2;
  display: flex;
  justify-content: flex-end;
}
.main-header {
  display: flex;
  justify-content: center;
  margin: 2rem 0;
}
.card-container {
  display: flex;
  justify-content: center;
  align-items: flex-end;
  flex-wrap: wrap;
  gap: 2rem;
  
  background-color: var(--blue);
}
/* ****************************** */
/* *** Content in logo wrapper *** */
/* ****************************** */

.logo-wrapper a {
  display: flex;
  align-items: center;
  transition: 300ms color;
  color: var(--light-red);
}
.logo-wrapper a:hover {
  color: var(--red);
}
.logo-wrapper p {
  font-size: 1.5rem;
}
.logo-wrapper i {
  font-size: clamp(3.5rem, 10vw, 4rem);
}

/* ****************************** */
/* *** Content in nav wrapper *** */
/* ****************************** */

/* child of nav-wrapper */
.nav-links {
  display:flex; 
  justify-content: space-around;
  white-space: nowrap;
  gap: 15px;
  flex-wrap: wrap;
}

/* ****************************** */
/* *** Content in nav wrapper *** */
/* ****************************** */

.signup {
  display: flex;
  justify-content: flex-end;
}
.signup a {
  background-color: var(--light-red);
  color: whitesmoke;
  border-radius: 2px;
  padding: 5px 20px;
  transition: 300ms background-color;
  text-align: center;
}
.signup i {
  font-size: 1.5rem;
}
.signup a:hover {
  background-color: var(--gray);
}

/* ************* */
/* *** Cards *** */
/* ************* */

.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  gap: 20px;
  
  background-color: var(--black);
  color: var(--white);
  padding: 20px;
  border-radius: 5px;
}
.card > *:nth-child(1) {
  background-color: var(--blue);
}
.card > *:nth-child(2) {
  background-color: var(--light-red);
}
.card > *:nth-child(3) {
  background-color: var(--blue);
}
.card-img-wrapper {
  max-width: 15rem;
}
```

### proof of work:

- (https://codepen.io/hyeju1996/pen/abVoPor)



# Jan 25,2022 Mobile First Design

Today we learn about code in mobile First Design. We code first is desktop design but later that changed to mobile in CSS work. 

Also, she show us what is CSS grid and layout and how to design our cards and layout with card. 

When I was take the lectire of lesson its give me Idea and I suddenly want a working on Project with website. My project is not yet but its give me Idea of how to design in.

Also, we designed Navigation bar too. 

## Challange:

My Challanged about I tried to understand flexbox on css and find img tools to working on and change mobile style way. Also, we working on alots of stuff so I want a keep looking at the codes we learn today. 

### Proof of work:

(https://codepen.io/hyeju1996/pen/zYPxWwE)


# Jan 26,2022 Web Design Patterns

We reviewd from yesterday work we also use flexbox yesterday and mobile thing. 

We also learn about live plugin and preiiter  and format on save with GitHub pages. 

## Issus:

I had issues about fontawesome icon. I tried send email and get the code but they said my email links are bad. 

## How I did solved

I send diffrent email and they just get me fontaweseome but me and Ashlyn got carious why my previous email addres is not working. Also, I checked just in case I used font awesome for last term in just in case 
