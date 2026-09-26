from pathlib import Path
p=Path("/mnt/data/vafibo_graduation.html")
text=p.read_text(encoding="utf-8")
text=text.replace("Vafibo","FIBO")
text=text.replace("vafibo","fibo")
p.write_text(text,encoding="utf-8")
print(f"[Download the FIBO HTML page](sandbox:{p})")
