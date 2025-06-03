# array_of_bad_words
JSON format

contains list of over **5,000 offensive, inappropriate, or profane words** in JSON format. It is designed for developers who need to implement text moderation, filtering, or censorship in applications such as chat systems, comment sections, forums, and games.

---

## 📁

- `bad_words_clean_5000.json`  
  → A JSON file containing a single array of bad words under the key `bad_words`.

**Example**
```
const fs = require('fs');

var bd = JSON.parse(fs.readFileSync('./bad_words_clean_5000.json')).bad_words;
function get_bad_words(text) {
  return bd.some(word => text.toLowerCase().includes(word));
}

console.log(get_bad_word("🥲"));
```

**GROUP ACTIONS**
👋 bye
✅ kick
❎ remove
