# Laddoo-proposal
const btn=document.getElementById("yes");
const result=document.getElementById("result");

btn.onclick=()=>{

result.style.display="block";

btn.innerHTML="❤️ Forever ❤️";

for(let i=0;i<80;i++){

let heart=document.createElement("div");

heart.innerHTML="❤️";

heart.style.position="fixed";
heart.style.left=Math.random()*100+"vw";
heart.style.top="-20px";
heart.style.fontSize=Math.random()*20+20+"px";
heart.style.transition="5s linear";

document.body.appendChild(heart);

setTimeout(()=>{

heart.style.top="100vh";

},50);

setTimeout(()=>{

heart.remove();

},5000);

}

}