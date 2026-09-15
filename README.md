
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Boys AI Prompts | Premium Gallery</title>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

:root {
  --bg: #0b0d12;
  --card: #151923;
  --card2: #1d2230;
  --text: #f7f7fb;
  --muted: #a6adbd;
  --accent: #8b5cf6;
  --accent2: #6d28d9;
  --border: #2b3140;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  background: var(--bg);
  color: var(--text);
  line-height: 1.6;
}

button, input, select {
  font: inherit;
}

button {
  cursor: pointer;
}

.hero {
  padding: 55px 20px 40px;
  text-align: center;
  background:
    radial-gradient(circle at 50% 0%, #3b1d68 0%, transparent 50%),
    var(--bg);
}

.hero h1 {
  font-size: clamp(30px, 5vw, 52px);
  line-height: 1.2;
  margin-bottom: 15px;
}

.hero h1 span {
  color: #b794ff;
}

.hero p {
  color: var(--muted);
  max-width: 680px;
  margin: auto;
  font-size: 16px;
}

.container {
  width: min(1180px, 92%);
  margin: auto;
}

.toolbar {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin: 25px 0;
}

.search,
.filter {
  background: var(--card);
  color: var(--text);
  border: 1px solid var(--border);
  border-radius: 10px;
  padding: 13px 15px;
  outline: none;
}

.search {
  flex: 1 1 240px;
  min-width: 0;
}

.filter {
  flex: 0 1 210px;
}

.search:focus,
.filter:focus {
  border-color: var(--accent);
}

.gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 24px;
  padding-bottom: 55px;
}

.prompt-card {
  background: var(--card);
  border: 1px solid var(--border);
  border-radius: 18px;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  min-width: 0;
  transition: transform .2s, border-color .2s;
}

.prompt-card:hover {
  transform: translateY(-4px);
  border-color: #7650bd;
}

.reference {
  width: 100%;
  aspect-ratio: 4 / 5;
  background: #252a36;
  overflow: hidden;
  position: relative;
}

.reference img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.reference-label {
  position: absolute;
  top: 12px;
  left: 12px;
  background: rgba(0,0,0,.65);
  padding: 5px 10px;
  border-radius: 6px;
  font-size: 12px;
  color: white;
}

.card-content {
  padding: 20px;
  display: flex;
  flex-direction: column;
  flex: 1;
}

.number {
  color: #b794ff;
  font-size: 12px;
  font-weight: bold;
  letter-spacing: 1px;
  text-transform: uppercase;
}

.card-title {
  font-size: 21px;
  line-height: 1.3;
  margin: 5px 0 10px;
}

.category {
  display: inline-block;
  width: fit-content;
  color: #d8c8ff;
  background: #2c2147;
  border: 1px solid #4b3470;
  border-radius: 30px;
  padding: 3px 10px;
  font-size: 12px;
  margin-bottom: 14px;
}

.prompt-box {
  background: var(--card2);
  border: 1px solid var(--border);
  border-radius: 10px;
  padding: 13px;
  color: #d9deea;
  font-size: 14px;
  max-height: 245px;
  overflow-y: auto;
  white-space: pre-wrap;
  word-break: break-word;
  flex: 1;
}

.copy-btn {
  border: none;
  background: linear-gradient(135deg, var(--accent), var(--accent2));
  color: white;
  padding: 13px;
  border-radius: 10px;
  margin-top: 16px;
  font-weight: bold;
  width: 100%;
}

.copy-btn:hover {
  filter: brightness(1.15);
}

.copy-btn.copied {
  background: #15803d;
}

.empty {
  display: none;
  text-align: center;
  color: var(--muted);
  padding: 45px 10px;
}

.footer {
  text-align: center;
  color: var(--muted);
  border-top: 1px solid var(--border);
  padding: 25px 15px;
  font-size: 14px;
}

@media (max-width: 600px) {
  .hero {
    padding: 38px 15px 30px;
  }

  .container {
    width: 94%;
  }

  .gallery {
    grid-template-columns: 1fr;
    gap: 20px;
  }

  .card-title {
    font-size: 20px;
  }

  .prompt-box {
    max-height: 280px;
  }
}
</style>
</head>

<body>

<header class="hero">
  <div class="container">
    <h1>Boys <span>AI Photo Prompts</span></h1>
    <p>
      Explore premium, detailed and copy-ready AI photography prompts.
      Choose a style, view the reference image and copy the complete prompt.
    </p>
  </div>
</header>

<main class="container">

  <div class="toolbar">
    <input
      class="search"
      id="search"
      type="search"
      placeholder="Search boys prompts..."
      aria-label="Search prompts"
    >

    <select class="filter" id="category" aria-label="Filter by category">
      <option value="all">All Categories</option>
      <option value="luxury">Luxury & Fashion</option>
      <option value="traditional">Pakistani Traditional</option>
      <option value="casual">Casual & Lifestyle</option>
      <option value="vehicles">Cars & Bikes</option>
      <option value="creative">Creative Portraits</option>
    </select>
  </div>

  <section class="gallery" id="gallery" aria-live="polite"></section>

  <p class="empty" id="empty">
    No prompts found. Try another search or category.
  </p>

</main>

<footer class="footer">
  © 2026 Boys AI Prompts — Premium AI Photography Collection
</footer>

<script>
const prompts = [

{
  id: 1,
  title: "Luxury Street Portrait",
  category: "luxury",
  image: "images/boy-01.jpg",
  prompt: `Create an ultra-realistic cinematic fashion portrait of an adult male model standing confidently on a modern luxury city street during golden hour. He wears a premium black oversized jacket, a clean white T-shirt, dark trousers and luxury sneakers. One hand is naturally inside the jacket pocket while the other remains relaxed. Natural upright posture, relaxed shoulders and a confident expression. Shot on a professional full-frame camera with an 85mm f/1.4 lens, shallow depth of field, sharp focus on the face, creamy background bokeh, soft golden-hour key light and subtle rim lighting. Modern architecture in the background, cinematic composition, realistic perspective, natural skin texture, detailed clothing fabric, warm cinematic color grading, realistic shadows, strong subject separation, premium editorial fashion photography, photorealistic, 4K, highly detailed.`
},

{
  id: 2,
  title: "Black Blazer Editorial",
  category: "luxury",
  image: "images/boy-02.jpg",
  prompt: `Create an ultra-realistic premium editorial portrait of an adult male model wearing a perfectly tailored black blazer, black trousers and a crisp white shirt. He stands beside a modern architectural wall with one hand in his trouser pocket and the other relaxed. Confident but natural facial expression, elegant masculine posture. Soft studio-style daylight, subtle shadows, 85mm portrait lens, shallow depth of field, sharp natural facial details, realistic skin pores and fabric texture. Sophisticated black and white fashion styling, luxury magazine composition, balanced framing, cinematic color grading, realistic proportions, professional fashion photography, photorealistic, 4K, no artificial skin, no distortion.`
},

{
  id: 3,
  title: "Pakistani White Shalwar Kameez",
  category: "traditional",
  image: "images/boy-03.jpg",
  prompt: `Create an ultra-realistic natural mobile-camera portrait of an adult Pakistani male wearing a clean, elegant white shalwar kameez. He is standing casually in a beautiful Pakistani outdoor courtyard with traditional architecture and soft natural daylight. His posture is relaxed, one hand resting naturally near his pocket and the other hanging comfortably. Preserve the subject's original face and identity if a reference photo is provided. Realistic skin texture, natural facial expression, detailed cotton fabric, authentic Pakistani clothing, soft shadows, realistic background, subtle depth of field, natural colors, no excessive retouching, no artificial-looking skin, high-quality photography, photorealistic, 4K.`
},

{
  id: 4,
  title: "Sky Blue Blazer Look",
  category: "luxury",
  image: "images/boy-04.jpg",
  prompt: `Create a highly realistic fashion portrait of an adult male model wearing a white shalwar kameez with a stylish sky-blue blazer. Add a subtle elegant chain and minimal accessories while keeping the overall look sophisticated. The subject stands in a modern outdoor setting with a softly blurred background. Natural confident pose, shoulders relaxed, slight body angle toward the camera, calm expression. Soft daylight, professional 85mm lens, realistic skin texture, detailed fabric, natural shadows, balanced exposure, premium Pakistani fashion editorial style, refined color grading, photorealistic, 4K, no facial distortion, no plastic skin.`
},

{
  id: 5,
  title: "Oversized Streetwear",
  category: "casual",
  image: "images/boy-05.jpg",
  prompt: `Create an ultra-realistic streetwear portrait of an adult male wearing an oversized charcoal T-shirt, loose-fit cargo trousers and clean modern sneakers. He stands on an urban sidewalk with modern buildings and subtle graffiti in the distance. One hand is holding a phone naturally while the other rests by his side. Relaxed confident expression, authentic street-fashion attitude, realistic proportions. Soft overcast daylight, 50mm lens, natural depth of field, sharp facial focus, detailed cotton texture, realistic shadows, neutral urban colors, professional streetwear photography, photorealistic, 4K, natural skin, no distortion.`
},

{
  id: 6,
  title: "Black Shirt Billiards",
  category: "casual",
  image: "images/boy-06.jpg",
  prompt: `Create a photorealistic cinematic portrait of an adult male wearing a premium oversized black shirt, dark trousers and a classic wristwatch inside an elegant billiards room. The subject stands beside a green billiards table, holding a cue naturally with one hand. Warm ambient lighting, subtle highlights on the face, realistic indoor shadows, luxurious lounge atmosphere, shallow depth of field, professional portrait photography, sharp natural facial details, detailed shirt fabric, realistic billiards table texture, balanced cinematic framing, deep but natural colors, 4K, no artificial skin, no distortion.`
},

{
  id: 7,
  title: "Classic Car Portrait",
  category: "vehicles",
  image: "images/boy-07.jpg",
  prompt: `Create an ultra-realistic lifestyle fashion photograph of an adult male standing beside a classic green Alfa Romeo in a beautiful outdoor location. He wears a stylish olive-green shirt, dark trousers and clean casual shoes. One hand rests naturally on the car while the other remains relaxed. Confident but natural pose, slight body angle toward the camera. Soft late-afternoon sunlight, realistic reflections on the car, professional 85mm lens, shallow depth of field, detailed fabric and skin texture, cinematic composition, premium automotive editorial photography, realistic shadows, photorealistic, 4K, no distortion.`
},

{
  id: 8,
  title: "Motorcycle Street Style",
  category: "vehicles",
  image: "images/boy-08.jpg",
  prompt: `Create a highly realistic cinematic portrait of an adult male standing beside a stylish modern motorcycle on a clean urban street. He wears a black leather jacket, fitted dark jeans, a plain T-shirt and modern sneakers. One hand rests naturally on the motorcycle handlebar while the other remains relaxed. Confident masculine pose, natural facial expression, realistic motorcycle details, soft evening light, subtle reflections, 50mm lens, shallow depth of field, sharp focus on the face, realistic skin and clothing texture, cinematic urban color grading, professional lifestyle photography, 4K, no distorted hands, no extra fingers.`
},

{
  id: 9,
  title: "Coffee Shop Portrait",
  category: "casual",
  image: "images/boy-09.jpg",
  prompt: `Create an ultra-realistic lifestyle portrait of an adult male sitting beside a large window in a modern cozy coffee shop. He wears a beige overshirt, a plain white T-shirt and dark trousers. He holds a takeaway coffee cup naturally and looks slightly toward the camera with a calm, thoughtful expression. Warm natural window light, soft shadows, realistic coffee shop background, wooden textures, 50mm lens, shallow depth of field, authentic skin texture, detailed clothing, natural hands, cinematic but realistic color grading, professional lifestyle photography, photorealistic, 4K, no artificial retouching.`
},

{
  id: 10,
  title: "Winter Pakistani Dressing",
  category: "traditional",
  image: "images/boy-10.jpg",
  prompt: `Create a photorealistic winter fashion portrait of an adult Pakistani male wearing a premium dark wool coat over a traditional shalwar kameez, with a simple textured scarf. He stands on a quiet winter street with soft fog and natural muted surroundings. Relaxed upright posture, hands naturally positioned, calm confident expression. Soft diffused daylight, realistic winter atmosphere, detailed wool and cotton fabric, natural facial texture, subtle depth of field, balanced composition, tasteful Pakistani winter styling, cinematic neutral color grading, professional fashion photography, 4K, realistic proportions, no distortion.`
},

{
  id: 11,
  title: "Luxury Hotel Lobby",
  category: "luxury",
  image: "images/boy-11.jpg",
  prompt: `Create an ultra-realistic luxury portrait of an adult male standing in an elegant five-star hotel lobby. He wears a tailored dark suit, a clean shirt and polished shoes. A sophisticated sofa, warm lights and elegant interior architecture appear softly in the background. The subject stands naturally with one hand in his pocket and a calm confident facial expression. Professional full-frame camera, 85mm lens, soft indoor lighting, realistic skin texture, detailed suit fabric, cinematic depth of field, premium editorial composition, natural shadows, refined color grading, photorealistic, 4K, no artificial-looking face, no distortion.`
},

{
  id: 12,
  title: "Rainy Night Portrait",
  category: "creative",
  image: "images/boy-12.jpg",
  prompt: `Create a cinematic ultra-realistic night portrait of an adult male standing on a modern city street during light rain. He wears a dark waterproof jacket over a plain shirt and dark trousers. Street lights and soft reflections on the wet road create a beautiful atmospheric background. The subject looks naturally toward the camera with a calm expression. Subtle rim lighting, realistic rain droplets, wet surface reflections, 85mm lens, shallow depth of field, sharp facial focus, natural skin texture, realistic clothing, cinematic cool and warm lighting balance, professional night photography, photorealistic, 4K, no distortion, no excessive effects.`
},

{
  id: 13,
  title: "Desert Adventure Look",
  category: "creative",
  image: "images/boy-13.jpg",
  prompt: `Create an ultra-realistic cinematic portrait of an adult male standing in a beautiful desert landscape during golden hour. He wears a premium beige overshirt, neutral trousers and clean boots. His posture is relaxed and confident, with one hand lightly touching his jacket and the other at his side. Soft golden sunlight, realistic sand textures, distant dunes, subtle wind in the clothing, natural skin details, professional full-frame camera, 85mm lens, beautiful background separation, warm cinematic color grading, authentic environmental lighting, premium outdoor fashion photography, photorealistic, 4K, no distortion.`
},

{
  id: 14,
  title: "Minimal Studio Portrait",
  category: "creative",
  image: "images/boy-14.jpg",
  prompt: `Create an ultra-realistic professional studio portrait of an adult male model against a simple warm-gray background. He wears a clean black crew-neck shirt and minimal accessories. The subject faces the camera with a relaxed and confident expression, shoulders naturally positioned. Use soft diffused studio lighting, subtle shadow falloff, realistic skin pores, detailed hair, natural eyes, professional 85mm portrait lens, sharp facial focus, clean composition, accurate facial proportions, premium magazine portrait style, natural color grading, photorealistic, 4K, no plastic skin, no distortion, no excessive smoothing.`
},

{
  id: 15,
  title: "Denim Casual Portrait",
  category: "casual",
  image: "images/boy-15.jpg",
  prompt: `Create a highly realistic casual fashion portrait of an adult male wearing a blue denim jacket over a plain white T-shirt, black jeans and clean sneakers. He stands beside a textured brick wall in a modern neighborhood. One hand is inside his jacket pocket while the other is relaxed. Natural smile, authentic body language, soft afternoon daylight, 50mm lens, realistic depth of field, detailed denim texture, natural skin and hair, realistic shadows, modern casual styling, balanced composition, professional street photography, photorealistic, 4K, no distortion, no artificial skin.`
},

{
  id: 16,
  title: "Traditional Kurta in Village",
  category: "traditional",
  image: "images/boy-16.jpg",
  prompt: `Create an ultra-realistic natural portrait of an adult Pakistani male wearing a simple light-colored traditional kurta shalwar in a peaceful village courtyard. The background includes authentic rural architecture, natural plants and a softly blurred environment. The subject stands casually with a relaxed posture and a natural facial expression. Soft morning sunlight, realistic rural atmosphere, detailed cotton fabric, authentic Pakistani styling, natural skin texture, professional mobile-camera photography, subtle depth of field, realistic shadows, natural colors, balanced framing, photorealistic, 4K, no excessive editing, no face distortion.`
},

{
  id: 17,
  title: "Luxury Sunglasses Look",
  category: "luxury",
  image: "images/boy-17.jpg",
  prompt: `Create an ultra-realistic premium fashion portrait of an adult male wearing a sophisticated black outfit, luxury sunglasses and a classic wristwatch. He stands beside a modern glass building with a softly blurred city background. One hand adjusts the sunglasses naturally while the other remains relaxed. Confident fashion-model stance, realistic body proportions, sharp focus on the face and accessories, professional 85mm lens, soft directional daylight, detailed clothing texture, natural skin, realistic reflections in the sunglasses, cinematic composition, premium editorial color grading, photorealistic, 4K, no distortion, no extra fingers.`
},

{
  id: 18,
  title: "Football Street Portrait",
  category: "casual",
  image: "images/boy-18.jpg",
  prompt: `Create a photorealistic lifestyle portrait of an adult male wearing a stylish football jersey, athletic trousers and clean sneakers on a modern outdoor sports ground. He stands naturally holding a football under one arm, looking confidently toward the camera. Realistic sports environment, subtle background blur, natural daylight, detailed jersey fabric, authentic facial expression, natural skin texture, professional 50mm camera lens, balanced composition, realistic shadows, crisp image quality, cinematic but natural color grading, professional sports lifestyle photography, 4K, no distorted hands, no extra limbs.`
},

{
  id: 19,
  title: "Traditional Eid Portrait",
  category: "traditional",
  image: "images/boy-19.jpg",
  prompt: `Create an ultra-realistic festive portrait of an adult Pakistani male wearing an elegant cream-colored shalwar kameez with a refined waistcoat. He stands in a beautifully decorated street during Eid celebrations, with tasteful lights and subtle festive decorations in the background. His pose is natural, with one hand near his waist and the other relaxed. Soft evening light, authentic Pakistani festive atmosphere, detailed traditional fabric, natural skin texture, realistic facial expression, professional portrait lens, shallow depth of field, balanced cinematic composition, natural colors, premium photography, photorealistic, 4K, no artificial skin, no distortion.`
},

{
  id: 20,
  title: "Cinematic Sad Portrait",
  category: "creative",
  image: "images/boy-20.jpg",
  prompt: `Create an ultra-realistic emotional cinematic portrait of an adult male standing alone beside a quiet window during a cloudy evening. He wears a simple dark shirt and trousers. His expression is thoughtful and slightly sad, with natural eyes and subtle emotion, without exaggerated tears. Soft window light falls gently across his face, creating realistic shadows and a calm atmospheric mood. Professional 85mm lens, shallow depth of field, sharp natural facial details, realistic skin texture, detailed fabric, muted cinematic color grading, authentic body language, professional portrait photography, photorealistic, 4K, no plastic skin, no distortion, no artificial expression.`
}

];

const gallery = document.getElementById("gallery");
const search = document.getElementById("search");
const category = document.getElementById("category");
const empty = document.getElementById("empty");

function escapeHTML(value) {
  return String(value).replace(/[&<>"']/g, char => ({
    "&": "&amp;",
    "<": "&lt;",
    ">": "&gt;",
    '"': "&quot;",
    "'": "&#039;"
  }[char]));
}

function categoryName(value) {
  const names = {
    luxury: "Luxury & Fashion",
    traditional: "Pakistani Traditional",
    casual: "Casual & Lifestyle",
    vehicles: "Cars & Bikes",
    creative: "Creative Portraits"
  };
  return names[value] || value;
}

function renderPrompts() {
  const term = search.value.trim().toLowerCase();
  const selected = category.value;

  const filtered = prompts.filter(item => {
    const searchable = (
      item.title + " " +
      item.prompt + " " +
      categoryName(item.category)
    ).toLowerCase();

    const matchesSearch = searchable.includes(term);
    const matchesCategory =
      selected === "all" || item.category === selected;

    return matchesSearch && matchesCategory;
  });

  gallery.innerHTML = "";
  empty.style.display = filtered.length ? "none" : "block";

  filtered.forEach(item => {
    const card = document.createElement("article");
    card.className = "prompt-card";

    card.innerHTML = `
      <div class="reference">
        <img
          src="${escapeHTML(item.image)}"
          alt="Reference photo for ${escapeHTML(item.title)}"
          loading="lazy"
          onerror="this.style.opacity='0.15'"
        >
        <span class="reference-label">REFERENCE PHOTO</span>
      </div>

      <div class="card-content">
        <span class="number">BOY PROMPT #${String(item.id).padStart(2, "0")}</span>
        <h2 class="card-title">${escapeHTML(item.title)}</h2>
        <span class="category">${escapeHTML(categoryName(item.category))}</span>

        <div class="prompt-box">${escapeHTML(item.prompt)}</div>

        <button class="copy-btn" type="button" data-id="${item.id}">
          📋 Copy Full Prompt
        </button>
      </div>
    `;

    gallery.appendChild(card);
  });
}

gallery.addEventListener("click", async event => {
  const button = event.target.closest(".copy-btn");
  if (!button) return;

  const item = prompts.find(
    prompt => prompt.id === Number(button.dataset.id)
  );

  if (!item) return;

  try {
    await navigator.clipboard.writeText(item.prompt);
  } catch (error) {
    const textArea = document.createElement("textarea");
    textArea.value = item.prompt;
    textArea.style.position = "fixed";
    textArea.style.opacity = "0";
    document.body.appendChild(textArea);
    textArea.focus();
    textArea.select();

    try {
      document.execCommand("copy");
    } catch (copyError) {
      alert("Please select and copy the prompt manually.");
    }

    textArea.remove();
  }

  const oldText = button.textContent;
  button.textContent = "✓ Prompt Copied!";
  button.classList.add("copied");

  setTimeout(() => {
    button.textContent = oldText;
    button.classList.remove("copied");
  }, 1800);
});

search.addEventListener("input", renderPrompts);
category.addEventListener("change", renderPrompts);

renderPrompts();
</script>

</body>
</html>
