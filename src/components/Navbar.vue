<template>
    <header>
        <nav class="navbar navbar-expand-lg ">
            <div class="container-fluid px-0">
                <a class="navbar-brand pe-4" href="#">
                    <img :src="logo" alt="Logo" width="80" height="28">
                </a>
                <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas"
                    data-bs-target="#offcanvasWithBothOptions" aria-controls="offcanvasWithBothOptions">
                    <img :src="menu" alt="Menu" width="35" height="20">
                </button>
                <div class="offcanvas offcanvas-end py-3 ps-2 offcanvas-size-sm" tabindex="-1" id="offcanvasWithBothOptions"
                    aria-labelledby="offcanvasWithBothOptionsLabel">
                    <div class="offcanvas-header">
                        <h5 class="offcanvas-title" id="offcanvasWithBothOptionsLabel"></h5>
                        <button type="button" class="btn" data-bs-dismiss="offcanvas" aria-label="Close">
                            <img :src="menuClose" alt="Close Menu">
                        </button>
                    </div>
                    <div class="offcanvas-body text-start">
                        <ul class="navbar-nav justify-content-start flex-grow-1 ">
                            <li class="nav-item dropdown pe-4">
                                <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown"
                                    aria-expanded="false">
                                    Features
                                </a>
                                <ul class="dropdown-menu">
                                    <li><a class="dropdown-item" href="#"><img :src="todoList" alt="TodoList"
                                                class="me-3">Todo List</a></li>
                                    <li><a class="dropdown-item" href="#"><img :src="calendar" alt="Calendar"
                                                class="me-3">Calendar</a></li>
                                    <li><a class="dropdown-item" href="#"><img :src="reminders" alt="Reminders"
                                                class="me-3">Reminders</a></li>
                                    <li><a class="dropdown-item" href="#"><img :src="planning" alt="Planning"
                                                class="me-3">Planning</a></li>
                                </ul>
                            </li>
                            <li class="nav-item dropdown">
                                <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown"
                                    aria-expanded="false">
                                    Company
                                </a>
                                <ul class="dropdown-menu">
                                    <li><a class="dropdown-item" href="#">History</a></li>
                                    <li><a class="dropdown-item" href="#">Our Team</a></li>
                                    <li><a class="dropdown-item" href="#">Blog</a></li>
                                </ul>
                            </li>
                            <li class="nav-item mx-3">
                                <a class="nav-link" href="#New">Careers</a>
                            </li>
                            <li class="nav-item mx-3">
                                <a class="nav-link" href="#">About</a>
                            </li>
                        </ul>
                        <ul class="navbar-nav justify-content-end flex-grow-1 ">
                            <li class="nav-item mx-3 btn login">
                                <a class="nav-link p-0" href="#New">Login</a>
                            </li>
                            <li class="nav-item mx-3 btn register px-4">
                                <a class="nav-link  p-0" href="#">Register</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </nav>
    </header>
</template>

<script setup>
import logo from '../assets/images/logo.svg'
import todoList from '../assets/images/icon-todo.svg'
import calendar from '../assets/images/icon-calendar.svg'
import planning from '../assets/images/icon-planning.svg'
import reminders from '../assets/images/icon-reminders.svg'
import menu from '../assets/images/icon-menu.svg'
import menuClose from '../assets/images/icon-close-menu.svg'
</script>

<style  scoped>
.register,.login{
   
    height: 2.5rem;
    border-radius: 10px;
    font-weight: 700;
}
.register{
    border: 1px solid;
}
a:hover{
    color: black;
}
.register:hover{
    border: 2px solid;
}
nav>*{
    font-weight: 700;
}
.offcanvas-size-sm{
    --bs-offcanvas-width: min(60vw, 250px) !important;
}
.navbar-toggler{
    border:  none ;
}
.navbar-toggler:focus,
.navbar-toggler:active,
.navbar-toggler-icon:focus {
    outline: none;
    box-shadow: none;
}
@media only screen and (max-width: 400px) {
  nav{
    padding: .9rem;
  }
}
</style>