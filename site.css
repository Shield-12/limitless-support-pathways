
const menu = document.querySelector('.menu');
const nav = document.querySelector('#navlinks');
menu?.addEventListener('click',()=>{
  const open = nav.classList.toggle('open');
  menu.setAttribute('aria-expanded', String(open));
});
const header = document.querySelector('.header');
if(header){
  let ticking=false;
  const update=()=>{
    const menuOpen = nav && nav.classList.contains('open');
    if(window.scrollY<=24 || menuOpen) header.classList.remove('header-hidden');
    else header.classList.add('header-hidden');
    ticking=false;
  };
  addEventListener('scroll',()=>{if(!ticking){requestAnimationFrame(update);ticking=true;}},{passive:true});
  update();
}
document.querySelectorAll('form[data-prototype]').forEach(form=>{
  form.addEventListener('submit',e=>{
    e.preventDefault();
    const status=form.querySelector('.form-status');
    if(status) status.textContent='Thank you. Your information has been received in this website prototype. A live site will need a secure submission service before publishing.';
    form.reset();
  });
});
