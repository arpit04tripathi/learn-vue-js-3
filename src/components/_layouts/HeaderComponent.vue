<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
    <header class="bg-gradient bg-light p-2 border-bottom border-dark border-3">
        <nav class="navbar navbar-expand-lg bg-body-tertiary">
            <div class="container-fluid">
                <RouterLink class="navbar-brand" to="/">
                    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="24" height="24" />
                    Learn vue js 3
                </RouterLink>
                <!-- <a class="navbar-brand" href="#">
                    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="24" height="24" />
                    Learn vue js 3
                </a> -->
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                    data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent"
                    aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                        <li class="nav-item">
                            <RouterLink class="nav-link" to="/"><span><i class="bi bi-house-door"></i> Home</span></RouterLink>
                        </li>
                        <li class="nav-item">
                            <RouterLink class="nav-link p-2" to="/about">About</RouterLink>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Link</a>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown"
                                aria-expanded="false">
                                Dropdown
                            </a>
                            <ul class="dropdown-menu">
                                <li><a class="dropdown-item" href="#">Action</a></li>
                                <li><a class="dropdown-item" href="#">Another action</a></li>
                                <li>
                                    <hr class="dropdown-divider">
                                </li>
                                <li><a class="dropdown-item" href="#">Something else here</a></li>
                            </ul>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link disabled" aria-disabled="true">Disabled</a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>

        <!-- <p>Header Component</p> -->
        <div class="bg-danger">
            <h3>
                <slot name="heading"></slot>
            </h3>
            <slot></slot>
        </div>
    </header>
</template>