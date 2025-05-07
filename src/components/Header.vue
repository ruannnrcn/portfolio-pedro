<template>

<header>
    <div class="container-header">
        <h1 class="h1-header">
            <slot name="title"></slot>
        </h1>
      <nav>
        <a href="#" id="about">Sobre</a>
        <a href="#">Projetos</a>
        <a href="#">Contato</a>
        <a href="#">Currículo</a>
        <a href="#">Github</a>
      </nav>
    </div>
  </header>
</template>

<style>
.container-header {
    width: 100%;
    height: 7rem;
    margin: 0 auto;
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    align-items: center;
    border-bottom: rgba(255, 255, 255, 0.1) solid 1px;
}

#about{
    border: none;
    background-color: var(--color-ascente);
    color: var(--text-color);
    font-size: 1.25rem;
    text-decoration: none;
    transition: 0.4s;
}

.h1-header {
    font-size: 2.5rem;
    color: var(--text-color);
}

nav {
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 20rem;
    gap: 1rem;

}

a{
    text-decoration: none;
    color: var(--text-color);
    transition: 0.4s;
    border-radius: 10px;
    padding: 0.5rem 1rem;
}

@media (hover: hover) {
  a:hover {
    background-color: var(--secundary-color);
  }
    #about:hover {
        background-color: var(--secundary-color);
    }
}
</style>
