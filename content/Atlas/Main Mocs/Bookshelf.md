---
M_Topics:
  - "[[Library]]"
  - "[[Home Page]]"
tags:
  - moc
---
>[!puzzle]- Book Category 1
>```dataview 
>table S_Topics, Author, ("![coverimg|100](" + Cover + ")") as Cover
>from #src/book-📚 and #Self-Dev OR #src/book-📚 and [[Self-Development]]
>where file.name != "{ Books To Read General MOC"
>where file.name != "Template Book"
>where file.name != "Bookshelf"
>```

> [!example] Full list
> ```dataview 
> list
> from #src/book-📚 
> where file.name != "{ Books To Read General MOC"
> where file.name != "Template Book"
> where file.name != "Bookshelf"
> ```
