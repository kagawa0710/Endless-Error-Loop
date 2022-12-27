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

