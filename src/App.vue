<template>
    <header>
        <nav class="navbar navbar-expand-lg bg-light">
        <div class="container-fluid">
            <a class="navbar-brand" href="#">메뉴</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
                <li class="nav-item">
                    <router-link to="/" class="nav-link active">메인</router-link>
                </li>
                <li class="nav-item">
                    <router-link to="/list" class="nav-link">목록</router-link>
                </li>
            </ul>
            </div>
        </div>
        </nav>
    </header>

    <main class="container mb-5 blog-list">
        <router-view :article="article"></router-view>
        <!-- <List :article="article" />  -->
        <!-- <div class="row mt-4">
            <div class="col">
                <div class="card p-0">
                    <p class="card-img-top"><img src="https://cdn.pixabay.com/photo/2017/02/20/18/03/cat-2083492_1280.jpg" alt="..."></p>
                    <div class="card-body">
                        <h5 class="card-title mt-2">Card title</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        <a href="#" class="card-link">Card link</a>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card p-0">
                    <p class="card-img-top"><img src="https://cdn.pixabay.com/photo/2016/11/29/01/10/kitten-1866475_1280.jpg" alt="..."></p>
                    <div class="card-body">
                        <h5 class="card-title mt-2">Card title</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content. Some quick example text to build on the card title and make up the bulk of the card's content. Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        <a href="#" class="card-link">Card link</a>
                    </div>
                </div>
            </div>
        </div>
        <div class="row mt-4">
            <div class="col">
                <div class="card p-0">
                    <p class="card-img-top"><img src="https://cdn.pixabay.com/photo/2019/11/08/11/56/kitten-4611189_1280.jpg" alt="..."></p>
                    <div class="card-body">
                        <h5 class="card-title mt-2">Card title</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content. Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        <a href="#" class="card-link">Card link</a>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card p-0">
                    <p class="card-img-top"><img src="https://cdn.pixabay.com/photo/2015/02/25/17/56/cat-649164_1280.jpg" alt="..."></p>
                    <div class="card-body">
                        <h5 class="card-title mt-2">Card title</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content. Some quick example text to build on the card title and make up the bulk of the card's content. Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        <a href="#" class="card-link">Card link</a>
                    </div>
                </div>
            </div>
        </div>

        <div class="row mt-4">
            <div class="col">
                <div class="card p-0">
                    <p class="card-img-top"><img src="https://cdn.pixabay.com/photo/2016/03/28/10/05/kitten-1285341_1280.jpg" alt="..."></p>
                    <div class="card-body">
                        <h5 class="card-title mt-2">Card title</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content. Some quick example text to build on the card title and make up the bulk of the card's content. Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        <a href="#" class="card-link">Card link</a>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card p-0">
                    <p class="card-img-top"><img src="https://cdn.pixabay.com/photo/2015/06/07/19/42/animal-800760_1280.jpg" alt="..."></p>
                    <div class="card-body">
                        <h5 class="card-title mt-2">Card title</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        <a href="#" class="card-link">Card link</a>
                    </div>
                </div>
            </div>
        </div> -->
    </main>

    <!-- <footer>
        footer
    </footer> -->

</template>

<script>
// import List from './components/List.vue';
import Blog from './assets/blog.js';

export default {
  name: 'App',
  data() {
    return {
        article: Blog,
    }
  },
  components: {
    // List: List,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.blog-list .row {
    display: flex;
}
.blog-list .card {
    height: 100%;
}
.blog-list .card-img-top {
    overflow: hidden;
    position: relative;
    width: 100%;
    padding-top: 65%; 
}
.blog-list .card-img-top img {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
}
.blog-list .card-body {
    display: flex;
    flex-direction: column;
}
.blog-list .card-link {
    margin-top: auto;
}

</style>
