# netflix-api

[Edit in StackBlitz next generation editor ⚡️](https://stackblitz.com/~/github.com/emrahkiziltan94/netflix-api)


https://api.themoviedb.org/3/trending/all/week?api_key=229df96d9cd7e64b815fad2f3de2890d&language=en-US

https://image.tmdb.org/t/p/w300/iADOJ8Zymht2JPMoy3R7xceZprc.jpg


const api = 'api_key=229df96d9cd7e64b815fad2f3de2890d';
// base URL of the site
const BaseURL = 'https://api.themoviedb.org/3';

const BannerURL = 'https://image.tmdb.org/t/p/original';
const ImgURL = 'https://image.tmdb.org/t/p/w300'; //change width here

//requestd for Movies data
const requests = {
  fetchTrending: `${BaseURL}/trending/all/week?${api}&language=en-US`,
  fetchNetflixOriginals: `${BaseURL}/discover/tv?${api}&with_networks=213`,
  fetchFamilyMovies: `${BaseURL}/discover/tv?${api}&with_genres=10751`,
  fetchComedyMovies: `${BaseURL}/discover/tv?${api}&with_genres=35`,
  fetchCrimeMovies: `${BaseURL}/discover/tv?${api}&with_genres=80`,
  fetchRomanceMovies: `${BaseURL}/discover/movie?${api}&with_genres=10749`,
  fetchDocumentaries: `${BaseURL}/discover/movie?${api}&with_genres=99`,
  fetchAnimeMovies: `${BaseURL}/discover/movie?${api}&with_genres=14`,
  fetchDramaMovies: `${BaseURL}/discover/movie?${api}&with_genres=18`,
  fetchMysteryMovies: `${BaseURL}/discover/movie?${api}&with_genres=9648`,
};