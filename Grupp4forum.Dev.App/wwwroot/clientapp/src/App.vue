<template>
    <div id="app">
        <img src="@/assets/flowertopleft.png" alt="Left Image" class="corner-image left-image" />
        <img src="@/assets/flowertopright.png" alt="Right Image" class="corner-image right-image" />
        <nav>
            <router-link to="/" class="btn custom-primary">Hem</router-link>
            <router-link to="/register" class="btn custom-primary">Registrera dig</router-link>
            <router-link to="/login" class="btn custom-primary">Logga in</router-link>
            <router-link to="/forum" class="btn custom-primary">Forum</router-link>
        </nav>
        <router-view />


    </div>
</template>

<style>
    #app {
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
    }

    nav {
        background-color: #F0F9E7;
        padding: 30px;
    }





    /* Custom button styles */
    .btn.custom-primary {
        background-color: #6ECB63;
        color: black;
        padding: 10px;
        border-radius: 5px;
        text-decoration: none;
        display: inline-block;
        margin: 10px;
        border-color: black;
    }

        .btn.custom-primary:hover {
            background-color: #5CA44A;
        }

    /*image*/

    .corner-image {
        position: absolute;
        height: auto;
    }

    .left-image {
        top: 0;
        left: 0;
    }

    .right-image {
        top: 0;
        right: 0;
    }
</style>