# how-to-use-clipboard-in-python-all-flatform
how to use clipboard in python all flatform

## Bước 1: cài các thư viện cần thiện cho việc copy, nếu là trên windows thì bỏ qua bước này
Bên dưới là cài cho ubuntu, nếu không làm bước này thì sau chạy code nó ghi là pyperclip không thích ứng cho hệ thống của bạn
```
sudo apt-get install xsel
sudo apt-get install xclip
```

## Bước 2: Tương tác clipboard sử dụng thư viện
### Cách 1: dùng pandas
Cài thư viện
```
pip install pandas
```
Gán content cho clipboard
```
content_input = data
df=pd.DataFrame([content_input])
df.to_clipboard(index=False,header=False)
```
### Cách 2: dùng clipboard
cài thư viện
```
pip install clipboard
```

Gán giá trị vào clipboard
```
clipboard.copy()
```

Lấy giá trị ra từ clipboard
```
ndung = clipboard.paste()
```
