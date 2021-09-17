- 👋 Hi, I’m @MO2KZ
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
MO2KZ/MO2KZ is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
-
kamiwhere: {
  expires_at: {gt: Time.now},   # lt, gte, lte also available
  orders_count: 1..10,          # equivalent to {gte: 1, lte: 10}
  aisle_id: [25, 30],           # in
  store_id: {not: 2},           # not
  aisle_id: {not: [25, 30]},    # not in
  user_ids: {all: [1, 3]},      # all elements in array
  category: {like: "%frozen%"}, # like
  category: /frozen .+/,        # regexp
  category: {prefix: "frozen"}, # prefix
  store_id: {exists: true},     # exists
  _or: [{in_stock: true}, {backordered: true}],
  _and: [{in_stock: true}, {backordered: true}],
  _not: {store_id: 1}           # negate a condition
}
kami
kami
