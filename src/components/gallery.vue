<meta charset="UTF-8">

<template>

<div id="gallery_container">
    <input
      id="gallery_searchbar"
      type="text"
      placeholder="ƒMƒƒƒ‰ƒŠ[‚ðŒŸõ"
      @input="UpdateCards"
      v-model="search_text"
    />
    <div id="galleries">
      <div class="card" v-for="card in disp_cards" :key="card.id">
        <img class="card_img" :src="card.image" />
        <div class="card_title">
          {{ card.title }}
        </div>
        <div class="card_description">
          {{ card.description }}
        </div>
      </div>
    </div>
  </div>

  </template>