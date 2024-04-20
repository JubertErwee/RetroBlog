<template>

    <div class="container">
        <header>
            <h1>Retro blog</h1>
            <nav>
                <ul class="nav">
                    <li class="nav-item">
                        <button type="button" class="btn btn-danger"><nuxt-link to="/" exact>Home</nuxt-link></button>
                    </li>
                    <li class="nav-item">
                        <button type="button" class="btn btn-warning"><nuxt-link to="/about">About</nuxt-link></button>
                    </li>
                    <!-- experiment -->
                    <li class="nav-item">
                        <button type="button" class="btn btn-danger"><nuxt-link to="/contact" exact>Contact</nuxt-link></button>
                    </li>
                    <!-- experiment -->
                    <!-- Add more navigation links here -->
                </ul>
            </nav>
        </header>
        
    </div>
    
    <div>
        <slot/>
    </div>
</template>