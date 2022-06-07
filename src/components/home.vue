<template>
  

  <!-- FOR LAPTOPES AND BIG SCREENS -->
  <div class="container laptopes">
    <div class="row row-cols-2">
      <div class="col">
        <h1>
          A person who reads lives a thousand lives <br />
          And the one who dosen't, lives only one!
        </h1>
        <h5>
          Explore the wonderful world of books and novels, find out what others
          are reading and exploring, know the views of others on a particular
          book, make friends and research together on same interests!
        </h5>
        <section class="buttons">
          <button class="btn btn-outline-success btn-lg" v-on:click="popup()">
            Review a Book
          </button>
          <button class="btn btn-outline-success btn-lg">Read reviews!</button>
        </section>
      </div>
      <div class="col img_cont" id="changeimg">
        <img
          src="https://p4.wallpaperbetter.com/wallpaper/427/799/775/library-artwork-books-wallpaper-preview.jpg"
          alt=""
        />
      </div>

      <div class="col form" id="form">
        <form>
          <div class="form-group">
            <label for="exampleInputEmail1">Email address: </label>
            <input
              type="email"
              class="form-control"
              id="email"
              aria-describedby="emailHelp"
              placeholder="Enter email"
            />
            <small id="emailHelp" class="form-text text-muted"
              >We'll never share your email with anyone else.</small
            >
          </div>
          <br />
          <div class="form-group">
            <label for="">Book Name: </label>
            <input type="text" id="bookname" class="form-control" />
          </div>
          <br />
          <div class="form-group">
            <label for="">Review: </label>
            <textarea type="text" id="bookreview" class="form-control" /></textarea>
            <small id="emailHelp" class="form-text text-muted"
              >Review the book within 500 words.</small
            >
          </div>
          <br />

          <button type="submit" class="btn btn-primary">Submit</button>
        </form>
      </div>

      <div class="col img_cont">
        <img
          src="http://initiativesmagazine.net/wp-content/uploads/2021/02/books-1.jpg"
          alt=""
        />
      </div>
      <div class="col">
        <h1>Explore your interests, read and research with other freaks!</h1>
        <h5 style="padding-bottom: 2%">Explore some of the common domains:</h5>
        <section class="buttons">
          <a class="btn btn-outline-primary" href="#" role="button"
            >Biographies</a
          >
          <a class="btn btn-outline-primary" href="#" role="button">Physics</a>
          <a class="btn btn-outline-primary" href="#" role="button"
            >Science Fiction</a
          >
          <a class="btn btn-outline-primary" href="#" role="button">Space</a>
          <a class="btn btn-outline-primary" href="#" role="button"
            >Self Help</a
          >
          <a class="btn btn-outline-primary" href="#" role="button"
            >Entrepreneurship</a
          >
          <a class="btn btn-outline-primary" href="#" role="button"
            >Stocks and Business</a
          >
        </section>
      </div>
      <hr />
      <hr />

      <div class="col books">
        <div class="card" style="width: 25rem">
          <img
            style="width: 50%"
            class="card_img img_cont"
            src="https://images-na.ssl-images-amazon.com/images/I/71VSswnjh9L.jpg"
            class="card-img-top"
            alt="..."
          />
          <div class="card-body">
            <h5 class="card-title">21 Lessons for the 21st century</h5>
            <p class="card-text img_cont">
              The third sequel of the series of books by Yuval Nova Harari,
              after the first- Sapiens and second- Homo Deus, this book focuses
              on the present of human civilization and beautifully connects the
              future aspects as well.
            </p>
            <a href="#" class="btn btn-primary">Explore!</a>
          </div>
        </div>
        <br />
        <div class="card" style="width: 25rem">
          <img
            style="width: 50%"
            class="card_img img_cont"
            src="https://images-na.ssl-images-amazon.com/images/I/71m-MxdJ2WL.jpg"
            class="card-img-top"
            alt="..."
          />
          <div class="card-body">
            <h5 class="card-title">Zero to one</h5>
            <p class="card-text img_cont">
              "Notes on Startups", one of the best book to explore the world of
              Entrepreneurship, for all the amateures and business freaks, this
              should be your first step.
            </p>
            <a href="#" class="btn btn-primary">Explore!</a>
          </div>
        </div>
      </div>

      <div class="col books">
        <div class="card" style="width: 25rem">
          <img
            style="width: 50%"
            class="card_img img_cont"
            src="https://images-na.ssl-images-amazon.com/images/I/814sKOe+BcL.jpg"
            class="card-img-top"
            alt="..."
          />
          <div class="card-body">
            <h5 class="card-title">Superintelligence</h5>
            <p class="card-text img_cont">
              All the AI freaks, this is the book, based on theoritical aspects
              of Artificial Intelligence and the researched views on the present
              and future of this domain. It's the book recommended by Bill Gates
              afterall.
            </p>
            <a href="#" class="btn btn-primary">Explore!</a>
          </div>
        </div>
        <br />
        <div class="card" style="width: 25rem">
          <img
            style="width: 50%"
            class="card_img img_cont"
            src="https://4.imimg.com/data4/KM/JQ/GLADMIN-10390523/images-jdbooks-1-90-6e2a88a33b4932fe9422804437eb9430-500x500.jpg"
            class="card-img-top"
            alt="..."
          />
          <div class="card-body">
            <h5 class="card-title">Think and grow rich</h5>
            <p class="card-text img_cont">
              This is the best ever self help book for all those who wants to
              know about mindset, Sub-conscious part of teh mind and ultimately
              the power of your brain and attitude in life to make it rich.
            </p>
            <a href="#" class="btn btn-primary">Explore!</a>
          </div>
        </div>
      </div>

      <hr />
      <hr />

      <div class="col">
        <h1>Entrepreneurship</h1>
        <h5>“The best way to predict the future is to create it.”</h5>
        <p class="textarea">
          Entrepreneurship is a kind of domain, about which most of the people
          are curious now-a-days. And why wouldn't they be, its a century formed
          on the back of so many Entrepreneurs like Elon Musk, Steve Jobs, Bill
          Gates, Mark Zukerberg, Larry page, Peter Theil and many more. They are
          not only transforming our future, but building it in such a way that
          it can only be imagined or seen in science fiction movies. <br />
          So, most important thing is- anyone can be an entrepreneur, by having
          nice ideas, business and entrepreneurial skills, execution plan and
          may or may not be a great and powerful team.
        </p>
      </div>
      <div class="col img_cont">
        <img
          style="height: 50%; width: 50%"
          class="col6"
          src="https://media.wired.com/photos/5932203658b0d64bb35d0024/master/w_2560%2Cc_limit/Musk-TA-492682182.jpg"
          alt=""
        />
        <img
          style="height: 50%; width: 49%"
          class="col6"
          src="https://images.unsplash.com/photo-1512820790803-83ca734da794?ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8ZW50cmVwcmVuZXVyc2hpcHxlbnwwfHwwfHw%3D&ixlib=rb-1.2.1&w=1000&q=80"
          alt=""
        />
        <img
          class="col6"
          src="https://images.unsplash.com/photo-1598301257982-0cf014dabbcd?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1000&q=80"
          alt=""
        />
        <img
          style="height: 40%; width: 50%"
          class="col6"
          src="https://www.washingtonian.com/wp-content/uploads/2015/09/stevejobs1.jpg"
          alt=""
        />
      </div>
      <hr />
      <hr />
      <div class="col">
        <h1>Space</h1>
        <h5>“I would like to die on Mars, just not on impact. -Elon Musk”</h5>
        <p class="textarea">
          Space is amongst those domains, which can transform the future of
          human civilization. As per the aims of Elon Musk, human civilization
          should be multi-planetary as soon as possible. And not only Elon (and
          his space company SpaceX), but many more leaders of the world are in
          the race of space exploration, like Blue origin, Virgin Galactic.
          <br />
          Space is one of the most liked domain for young minds to explore and
          learn various things about astrology. The Earth is the cradle of
          humanity, but mankind cannot stay in the cradle forever.
        </p>
      </div>
      <div class="col img_cont">
        <img
          style="height: 50%; width: 50%"
          class="col6"
          src="https://images.theconversation.com/files/405990/original/file-20210611-13-pcdwbd.jpg?ixlib=rb-1.1.0&q=45&auto=format&w=1200&h=1200.0&fit=crop"
          alt=""
        />
        <img
          style="height: 50%; width: 49%"
          class="col6"
          src="https://thumbor.forbes.com/thumbor/960x0/https%3A%2F%2Fspecials-images.forbesimg.com%2Fdam%2Fimageserve%2F765877054%2F960x0.jpg%3Ffit%3Dscale"
          alt=""
        />
        <img
          style="height: 50%; width: 70%"
          class="col6"
          src="https://media-cldnry.s-nbcnews.com/image/upload/t_fit-760w,f_auto,q_auto:best/newscms/2018_34/2541606/180823-space-books-main-art-mn-1125.jpg"
          alt=""
        />
      </div>
      <hr />
      <hr />
      <div class="col">
        <h1>Biographies</h1>
        <h5>
          “Read biographies, for that is life without theory. -Benjamin
          Disraell”
        </h5>
        <p class="textarea">
          Biographies are really important to read, because these books tell you
          all about a persons life, how he/she succeeded in the life, more
          importantly how they tackled various hurdles and many more. A person
          who you think as your role model and wanted to be like him/her, either
          professionally of generally as a person, then biography of that great
          personalty can teach you all the things and gives you a chance to dive
          deep into their lives to explore and learn tons of life lessons.
        </p>
      </div>
      <div class="col img_cont">
        <img
          style="height: 50%; width: 30%"
          class="col6"
          src="https://3.imimg.com/data3/VM/WT/MY-12313319/kalam-500x500.jpeg"
          alt=""
        />
        <img
          style="height: 50%; width: 30%"
          class="col6"
          src="https://images.gr-assets.com/books/1511288482l/11084145.jpg"
          alt=""
        />
        <img
          style="height: 50%; width: 30%"
          class="col6"
          src="https://i.gr-assets.com/images/S/compressed.photo.goodreads.com/books/1328011405l/10884.jpg"
          alt=""
        />
        <img
          style="height: 50%; width: 90%"
          class="col6"
          src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQWpT2WShNnkfOjQ60cYXaJuC7buSSoa7pG1A&usqp=CAU"
          alt=""
        />
      </div>
      <hr />
      <hr />
      <div class="col">
        <h1>Self-Help</h1>
        <h5>“Books that talks about life through beautiful fables”</h5>
        <p class="textarea">
          A successful self-help book author establishes a relationship with you
          by writing a book that's relatively easy to use, makes you feel that
          there's hope for you, shows you that the author understands your
          problems, and gives you at least some advice for life right away.
          These books encourages you to focus on your goals, figure out
          strategies on achieving those goals, overcoming obstacles that delay
          your achievements, and staying inspired all the way long.
        </p>
      </div>
      <div class="col img_cont">
        <img
          style="height: 50%; width: 30%"
          class="col6"
          src="https://images-na.ssl-images-amazon.com/images/I/41+eK8zBwQL._SX319_BO1,204,203,200_.jpg"
          alt=""
        />
        <img
          style="height: 50%; width: 30%"
          class="col6"
          src="https://images-na.ssl-images-amazon.com/images/I/61Iz2yy2CKL.jpg"
          alt=""
        />
        <br />
        <img
          style="height: 50%; width: 30%"
          class="col6"
          src="https://images-na.ssl-images-amazon.com/images/I/51-nXsSRfZL._SX328_BO1,204,203,200_.jpg"
          alt=""
        />
        <img
          style="height: 50%; width: 30%"
          class="col6"
          src="https://m.media-amazon.com/images/I/51iGkLC6jhL.jpg"
          alt=""
        />
      </div>
    </div>
  </div>

  <!-- FOR PHONES -->
  <div class="container phones" style="width: 200%">
    <div class="col">
      <h1>
        A person who reads lives a thousand lives <br />
        And the one who dosen't, lives only one!
      </h1>
      <h5>
        Explore the wonderful world of books and novels, find out what others
        are reading and exploring, know the views of others on a particular
        book, make friends and research together on same interests!
      </h5>
      <section class="buttons">
        <a href="#" type="button" class="btn btn-outline-success btn-lg"
          >Review a book!</a
        >
        <a href="#" type="button" class="btn btn-outline-success btn-lg"
          >Read reviews!</a
        >
      </section>
    </div>

    <div class="col">
      <h1>Explore your interests, read and research with other freaks!</h1>
      <h5 style="padding-bottom: 2%">Explore some of the common domains:</h5>
      <section class="buttons">
        <a class="btn btn-outline-primary" href="#" role="button"
          >Biographies</a
        >
        <a class="btn btn-outline-primary" href="#" role="button">Physics</a>
        <a class="btn btn-outline-primary" href="#" role="button"
          >Science Fiction</a
        >
        <a class="btn btn-outline-primary" href="#" role="button">Space</a>
        <a class="btn btn-outline-primary" href="#" role="button">Self Help</a>
        <a class="btn btn-outline-primary" href="#" role="button"
          >Entrepreneurship</a
        >
        <a class="btn btn-outline-primary" href="#" role="button"
          >Stocks and Business</a
        >
      </section>
    </div>
    <hr />
    <div class="col">
      <h1>Entrepreneurship</h1>
      <h5>“The best way to predict the future is to create it.”</h5>
      <p>
        Entrepreneurship is a kind of domain, about which most of the people are
        curious now-a-days. And why wouldn't they be, its a century formed on
        the back of so many Entrepreneurs like Elon Musk, Steve Jobs, Bill
        Gates, Mark Zukerberg, Larry page, Peter Theil and many more. They are
        not only transforming our future, but building it in such a way that it
        can only be imagined or seen in science fiction movies. <br />
        So, most important thing is- anyone can be an entrepreneur, by having
        nice ideas, business and entrepreneurial skills, execution plan and may
        or may not be a great and powerful team.
      </p>
    </div>
    <div class="col">
      <h1>Space</h1>
      <h5>“I would like to die on Mars, just not on impact. -Elon Musk”</h5>
      <p>
        Space is amongst those domains, which can transform the future of human
        civilization. As per the aims of Elon Musk, human civilization should be
        multi-planetary as soon as possible. And not only Elon (and his space
        company SpaceX), but many more leaders of the world are in the race of
        space exploration, like Blue origin, Virgin Galactic. <br />
        Space is one of the most liked domain for young minds to explore and
        learn various things about astrology. The Earth is the cradle of
        humanity, but mankind cannot stay in the cradle forever.
      </p>
    </div>
    <div class="col">
      <h1>Biographies</h1>
      <h5>
        “Read biographies, for that is life without theory. -Benjamin Disraell”
      </h5>
      <p>
        Biographies are really important to read, because these books tell you
        all about a persons life, how he/she succeeded in the life, more
        importantly how they tackled various hurdles and many more. A person who
        you think as your role model and wanted to be like him/her, either
        professionally of generally as a person, then biography of that great
        personalty can teach you all the things and gives you a chance to dive
        deep into their lives to explore and learn tons of life lessons.
      </p>
    </div>
    <div class="col">
      <h1>Self-Help</h1>
      <h5>“Books that talks about life through beautiful fables”</h5>
      <p>
        A successful self-help book author establishes a relationship with you
        by writing a book that's relatively easy to use, makes you feel that
        there's hope for you, shows you that the author understands your
        problems, and gives you at least some advice for life right away. These
        books encourages you to focus on your goals, figure out strategies on
        achieving those goals, overcoming obstacles that delay your
        achievements, and staying inspired all the way long.
      </p>
    </div>
  </div>

  <script
    src="https://code.jquery.com/jquery-3.5.1.slim.min.js"
    integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj"
    crossorigin="anonymous"
  ></script>
  <script
    src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js"
    integrity="sha384-9/reFTGAW83EW2RDu2S0VKaIzap3H66lZH81PoYlFhbGU+6BZp6G7niu735Sk7lN"
    crossorigin="anonymous"
  ></script>
  <script
    src="https://cdn.jsdelivr.net/npm/bootstrap@4.6.0/dist/js/bootstrap.min.js"
    integrity="sha384-+YQ4JLhjyBLPDQt//I+STsc9iw4uQqACwlvpslubQzn4u2UU2UFM80nGisd026JF"
    crossorigin="anonymous"
  ></script>
</template>

<script>
export default {
  name: 'Home',
  props: {
    data: String,
    msg: String,
  },
  data() {
    return {
      name: 'Sahil',
      a: 20,
      b: 30,
      show: true,
    };
  },
  methods: {
    hello() {
      alert("Hii there, how's going?");
    },
    popup() {
      const img = document.querySelector('#changeimg');
      img.style.display="none";

      const form = document.querySelector('#form');
      form.style.display="inline";
    },
    changeName() {
      if (this.name == 'Sahil') {
        this.name = 'Tanishq';
      } else {
        this.name = 'Sahil';
      }
    },
    changeStyle() {
      this.show = !this.show;
    },
  },
};
</script>

<style scoped>
@media (max-width: 500px) {
  .laptopes {
    display: none;
  }
}

@media (max-width: 1000px) {
  hr {
    display: none;
  }
  .img_cont {
    display: none;
  }
}

@media (min-width: 500px) {
  .phones {
    display: none;
  }
}

body {
  background-repeat: repeat-x;
}

nav {
  position: fixed;
}

.col {
  padding: 3%;
  width: 45%;
}

img {
  border-radius: 5%;
  width: 100%;
  padding-top: 13%;
}

h1 {
  padding-left: 8%;
  padding-top: 8%;
  padding-right: 8%;
  text-align: center;
}
h5 {
  padding-left: 8%;
  padding-bottom: 2%;
  padding-right: 8%;
  text-align: center;
}

.btn {
  margin: 0.5%;
}

.buttons {
  text-align: center;
}

.col6 {
  padding: 1%;
  width: 45%;
}

.card {
  text-align: center;
  border-radius: 5%;
  border: 0ch;
}

.card {
  border: solid rgba(0, 0, 0, 0.479) 0.2ch;
  transition: 0.2s;
  margin-left: 100px;
}
.card:hover {
  background: rgba(0, 255, 242, 0.548);
  border: solid rgba(0, 255, 242, 0.548) 0.2ch;
}

.card_img {
  padding: 5%;
  width: 13rem;
}

.textarea {
  padding: 50px;
}

.form-control {
  width: 50px;
}

#bookname,
#bookreview,
#email {
  width: 50%;
}

#bookreview {
  width: 90%;
  height: 500%;
}

form {
  border: 5px solid #ced4da;
  border-radius: 10px;
  padding: 10px;
  text-align: left;
  margin-top: 50px;
}

.form{
  display: none;
  
}
</style>
