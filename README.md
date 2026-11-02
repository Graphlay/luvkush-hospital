# Luv Kush Hospital – Website (by Graphlay)

## Folder mein kya hai
- `index.html` – poori website (design + code ek hi file mein)
- `assets/img/` – doctors, building aur hospital ki photos
- `assets/video/` – 6 hospital videos (web ke liye compress kiye hue)

## Demo mode (abhi chalu hai)
`index.html` mein neeche `CONFIG` dhoondhiye:

```js
demo: true,
demoUntil: "2026-11-09T23:59:59+05:30",
```

Demo mode mein ye hota hai:
- Upar laal patti dikhti hai: "Demo website prepared by Graphlay".
- Poori site par halka "GRAPHLAY DEMO" watermark hota hai.
- Booking aur WhatsApp button dabane par "This is a preview" popup khulta hai, jisme Graphlay se baat karne ka button hai.
- Emergency call button hamesha hospital ke asli number (81077 81966) par jaata hai, taaki kisi mareez ki call galat jagah na jaye.
- `demoUntil` ki tareekh ke baad site band ho jaati hai aur "This preview has ended" dikhta hai.
- Google is demo ko search mein nahi dikhayega (`noindex`).

## Payment ke baad live karna
1. `index.html` mein `demo: true` ko `demo: false` kar dijiye.
2. `<head>` mein `<meta name="robots" content="noindex, nofollow">` wali line delete kar dijiye.
3. Hospital ka asli logo mile to header ka SVG logo badal dijiye (code mein comment laga hai).
4. Domain (jaise luvkushhospital.in) jod dijiye.

## Hosting ke baare mein
- GitHub Pages par free plan mein repo **public** rakhni padti hai, yani koi bhi code dekh kar `demo: false` kar sakta hai.
- Demo ke liye **Netlify** (netlify.com/drop par folder drag karke) behtar hai, kyunki wahan code kisi ko nahi dikhta.
- Payment ke baad final site GitHub Pages ya Netlify, kahin bhi daal sakte hain.
