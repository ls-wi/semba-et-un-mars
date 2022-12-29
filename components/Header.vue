<template>
  <nav class="nav">
    <div>
      <img class="logo" src="../assets/images/logoT.png" />
    </div>

    <ul class="nav">
      <li class="link">
        <div class="dropdown inline-block relative">
          <button
            class="
              link
              font-semibold
              py-2
              px-4
              rounded
              inline-flex
              items-center
            "
          >
            <span class="mr-1">Evènements</span>
            
            <svg
              class="fill-current h-4 w-4"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 20 20"
            >
              <path
                d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"
              />
            </svg>
          </button>
          <ul class="dropdown-menu absolute hidden text-gray-700 pt-1">
            <li class="">
              <a
                class="
                  rounded-t
                  bg-[#faec92]
                  hover:bg-white
                  py-2
                  px-4
                  block
                  whitespace-no-wrap
                "
                href="#"
                >Off Angouleme</a
              >
            </li>
            <li class="">
              <a
                class="
                  bg-[#faec92]
                  hover:bg-white
                  py-2
                  px-4
                  block
                  whitespace-no-wrap
                "
                href="#"
                >Off du Tertre</a
              >
            </li>
            <li class="">
              <a
                class="
                  bg-[#faec92]
                  hover:bg-white
                  py-2
                  px-4
                  block
                  whitespace-no-wrap
                "
                href="#"
                >Olympique-Bar</a
              >
            </li>
            <li class="">
              <a
                class="
                  bg-[#faec92]
                  hover:bg-white
                  py-2
                  px-4
                  block
                  whitespace-no-wrap
                "
                href="#"
                >P'Art'Ouze</a
              >
            </li>
            <li class="">
              <a
                class="
                  bg-[#faec92]
                  hover:bg-white
                  py-2
                  px-4
                  block
                  whitespace-no-wrap
                "
                href="#"
                >Route de la Bière</a
              >
            </li>
            <li class="">
              <a
                class="
                  bg-[#faec92]
                  hover:bg-white
                  py-2
                  px-4
                  block
                  whitespace-no-wrap
                "
                href="#"
                >Route du shot</a
              >
            </li>
            <li class="">
              <a
                class="
                  bg-[#faec92]
                  hover:bg-white
                  py-2
                  px-4
                  block
                  whitespace-no-wrap
                "
                href="#"
                >Route du short</a
              >
            </li>
            <li class="">
              <a
                class="
                  bg-[#faec92]
                  hover:bg-white
                  py-2
                  px-4
                  block
                  whitespace-no-wrap
                "
                href="#"
                >Seumfest</a
              >
            </li>
            <li class="">
              <a
                class="
                  bg-[#faec92]
                  hover:bg-white
                  py-2
                  px-4
                  block
                  whitespace-no-wrap
                "
                href="#"
                >SeumSquat</a
              >
            </li>
            <li class="">
              <a
                class="
                  bg-[#faec92]
                  hover:bg-white
                  py-2
                  px-4
                  block
                  whitespace-no-wrap
                "
                href="#"
                >Soirée SEUM</a
              >
            </li>
            <li class="">
              <a
                class="
                  rounded-b
                  bg-[#faec92]
                  hover:bg-white
                  py-2
                  px-4
                  block
                  whitespace-no-wrap
                "
                href="#"
                >Tournoi de foot Interbar</a
              >
            </li>
          </ul>
        </div>
      </li>
      <li class="link               
              font-semibold
              py-2
              px-4">
        <a href="#">Qui sommes nous ?</a>
      </li>

      <li class="link               
              font-semibold
              py-2
              px-4">
        <a href="#">Nous contacter</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
.dropdown:hover .dropdown-menu {
  display: block;
}

nav {
  border-bottom: blue 3px solid;
  padding:1px;
  z-index:500;
}

nav ul {
  border-bottom: blue 2px solid;
}
</style>