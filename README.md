- 👋 Hi, I’m @conyo2
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
conyo2/conyo2 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
const { Strategy } = require('zenbot');

module.exports = new Strategy({
  name: 'example-strategy',
  description: 'An example strategy for Zenbot',
  getOptions: () => ({
    option1: {
      type: 'string',
      default: 'default-value',
      description: 'Option 1 description'
    },
    option2: {
      type: 'bool',
      default: true,
      description: 'Option 2 description'
    }
  }),
  calculate: function (s) {
    // Burada hesaplama yapılır
  },
  onPeriod: function (s, cb) {
    // Burada al-sat kararları alınır
    // Al-sat işlemi gerçekleştirilir
  }
});
