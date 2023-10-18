<template>
    <div class="movie-list-items">

        <li class="movie-list-item d-flex justify-content-between" v-for="movie in movies">
            <span class="text-align-center">{{movie.name}}</span>
            <div class="movie-list-icons d-flex justify-content-between">
                <input type="number" class="outline-none" :value="movie.viewers">
                <i class="d-flex justify-content-evely">
                    <button class="btn btn-danger fa fa-trash"></button>
                    <button class="btn btn-success fa fa-cookie"></button>
                    <button class="fa fa-star btn btn-star"></button>
                </i>
            </div>
        </li>

    </div>
</template>
<script>
export default {
    data() {
        return {
            movies: [
                {name: `Rasulbek Hakimov`, viewers: 777},
                {name: `Rasulbek Hakimov`, viewers: 666},
            ]
        }
    }
}
</script>
<style scoped>
.btn-star,
.btn-star:hover {
    color: orange;
}

.fa-cookie,
.fa-cookie:hover {
    color: orange;
}

.movie-list-items {
    margin-top: 2rem;
    padding: 1.5rem;
    background-color: #fcfaf5;
    border-radius: 4px;
    box-shadow: 15px 15px 15px rgba(0, 0, 0, 0.15);
}
.movie-list-item {
    padding: 1.5rem;
    background-color: #fcfaf5;
    border-radius: 4px;
    box-shadow: 15px 15px 15px rgba(0, 0, 0, 0.15);
    border-bottom: 1px solid black;
}
.movie-list-item:last-child{
    border: none;
}
.movie-list-icons{
    gap: 30px;
}
input {
    text-align: center;
    outline: none;
    border: none;
}
</style>