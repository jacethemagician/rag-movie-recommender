自我数据集design
- 加plot column（source：wiki）
- 通过plot fill summary column
- 翻译成英文
- 对没有input做人工fill
- priority改成high, med low
- rating 做成 int
- comment拆解成多个评价col，如音乐，script等
- 增加genre tag

自己数据库vectordb
- genre
- actors
- director
- keyword w/ comment
- categorical rating

总db
- name
- genres
- actors
- director
- plot summary
- overall rating

1. 自己的数据集转化成vectordb的数据格式：keyword用ai生成, rating直接取
2. "recent, fun, comedy" ->query 自己数据库vectordb
？（rating有什么用？能不能和keyword结合，比如不好的rating的keyword也能给信息）->movie list
3. Prompt（movie list） -> query 总数据库 -> similarity rank
- prompt需要设计
- 1