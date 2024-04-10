# Get Grass With WebUI

**This is a python tools for get grass score with multi accounts.**

![img.png](img.png)

### **Run Python script alone**
1. ```pip3 install -r requirements.txt```
2. ```python3 main.py```
3. 浏览器访问`http://127.0.0.1:8000`
4. 点击上传文件 上传编辑好的 `account.txt`

### **Docker Compose **
1. `git clone https://github.com/Confusion-ymc/GetGrassWebUI.git`
2. `docker compose up --build -d`
3. GUI deployed at: `http://{容器ip}:8000`
4. Upload file to add multiple accounts `account.txt`

### About the `account.txt` file format
- No proxy configuration
   - **Each line is an account configuration**
   - **If there is no proxy, `user_id` is directly in one line, ----- the format is `5242367b-d366-1234-987a-9ebd303fa8f5`**
- Configure proxy
   - **If you use a socks proxy, add `== proxy connection` at the end - the format is `5242367b-d366-1258-987a-9ebd303fa8f5==socks5://proxy.com:1080`**
   - **If you use a http proxy, add `== proxy connection` at the end - the format is `5242367b-d366-1258-987a-9ebd303fa8f5==http://user:password@proxy.com:port`**

