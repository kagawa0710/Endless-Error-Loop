# Neko Hacker - Endless Error Loop feat. ななひら

---

```
TRY / EXCEPT
    よくあるError
TRY / EXCEPT
    見たことないError
TRY / EXCEPT
    不死身のError
TRY / EXCEPT
    名も無きError
```

``` mermaid
graph TD
  ST((Start))       --> Try1{TRY1}
  Try1 -- Success   --> Try2{TRY2}
  Try1 -- error     --> except1[よくあるError]
  Try2 -- Success   --> Try3{TRY3}
  Try2 -- error     --> except2[見たことないError]
  Try3 -- Success   --> Try4[TRY4]
  Try3 -- error     --> except3[不死身のError]
  Try4 -- Success   --> Next[Next]
  Try4 -- error     --> except4[名も無きError]
```

---
```
if status == "解決しない":
  print("発狂しちゃう")
elif status == "別のエラーが出る":
  print("3日間は寝込んじゃう")
elif status == "解決方法見つける":
  print("英語は全く読めない")
```

```mermaid
graph TD
  ST(Start)             --> Check1{"status == #quot;解決しない#quot;"}
  Check1    -- True     --> Output1["print(#quot;発狂しちゃう#quot;)"]
  Check1    -- False    --> Check2{"status == #quot;別のエラーが出る#quot;"}
  Check2    -- True     --> Output2["print(#quot;3日間は寝込んじゃう#quot;)"]
  Check2    -- False    --> Check3{"status == #quot;解決方法見つける#quot;"}
  Check3    -- True     --> Output3["print(#quot;英語は全く読めない#quot;)"]
  
```
---
