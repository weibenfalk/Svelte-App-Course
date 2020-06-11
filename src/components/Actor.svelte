<script>
  import { POSTER_SIZE, IMAGE_BASE_URL } from '../config';
  const noImage = '/images/no_image.jpg';

  export let actor;
</script>

<div class="wrapper">
  <img
    src={actor.profile_path ? `${IMAGE_BASE_URL}${POSTER_SIZE}${actor.profile_path}` : noImage}
    alt="actorthumb" />
  <span class="name">{actor.name}</span>
  <span class="character">{actor.character}</span>
</div>

<style>
  .wrapper {
    color: #fff;
    background: #1c1c1c;
    border-radius: 20px;
    padding: 5px;
    text-align: center;
  }

  img {
    display: block;
    width: 100%;
    height: 200px;
    object-fit: cover;
    border-radius: 15px;
  }

  .name {
    display: block;
    font-size: 18px;
    margin: 10px 0 0 0;
  }

  .character {
    display: block;
    font-size: 16px;
    margin: 0 0 10px 0;
  }
</style>
