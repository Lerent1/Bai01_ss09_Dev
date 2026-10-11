# Bài 1: Kiểm tra cài đặt Docker Engine và chạy Container Hello-World

## 1. Mục tiêu

- Kiểm tra phiên bản Docker CLI.
- Kiểm tra kết nối tới Docker Daemon.
- Chạy container `hello-world`.
- Lưu kết quả vào file `REPORT.md`.

## 2. Các lệnh thực hiện

```bash
docker version
docker info
docker run hello-world
```

## 3. Lưu kết quả vào REPORT.md

Chạy các lệnh sau tại thư mục `homework/session_09/ex1/`:

```bash
{
  echo "# REPORT - Docker Engine"
  echo
  echo "## 1. Docker Version"
  echo '```text'
  docker version 2>&1
  echo '```'
  echo
  echo "## 2. Docker Info"
  echo '```text'
  docker info 2>&1
  echo '```'
  echo
  echo "## 3. Docker Run Hello-World"
  echo '```text'
  docker run hello-world 2>&1
  echo '```'
} > REPORT.md
```

## 4. Kiểm tra kết quả

```bash
cat REPORT.md
```

Kết quả mong đợi khi chạy `docker run hello-world`:

```text
Hello from Docker!
This message shows that your installation appears to be working correctly.
```

## 5. Nộp bài lên GitHub

Đường dẫn: `homework/session_09/ex1/REPORT.md`

```bash
git add homework/session_09/ex1/REPORT.md
git commit -m "Add Docker hello-world report"
git push origin main
```

