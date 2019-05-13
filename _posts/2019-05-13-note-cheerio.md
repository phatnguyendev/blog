---
layout: post
title: Take note with Cheerio
subtitle: Note về cheerio trong NodeJS
bigimg: /img/path.jpg
tags: [cheerio, nodeJS]
---
# Làm quen với Cheerio bằng crawler
Đây là note những lưu ý hay ho trong lúc sử dụng cheerio
## Tìm kiếm
Sử dụng $(body).find("a.title") trong đó
>body: html source được lấy về
>a: tên tag 
>.title: truy cập đến class (# cho id)

## Dùng vòng lặp
Sử dụng .each(function(i,e) {
	với i là biến chạy,
	e tượng trưng cho obj
})

## Lấy các thứ trong tag
ví dụ muốn lấy nội dung của tag a
$(this).text()
muốn lấy thuộc tính của a (như href)
e["attribs"]["href"]
