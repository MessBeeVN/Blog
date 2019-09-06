---
title: "Liên hệ"
permalink: "/lien-he.html"
---

<form action="https://formspree.io/{{site.email}}" method="POST">    
<p class="mb-4">Nhập lời nhắn bạn muốn gửi cho {{site.name}}. Chúng tôi sẽ liên hệ lại sớm nhất có thể!</p>
<div class="form-group row">
<div class="col-md-6">
<input class="form-control" type="text" name="name" placeholder="Họ và tên*" required>
</div>
<div class="col-md-6">
<input class="form-control" type="email" name="_replyto" placeholder="Địa chỉ email*" required>
</div>
</div>
<textarea rows="8" class="form-control mb-3" name="message" placeholder="Lời nhắn*" required></textarea>    
<input class="btn btn-success" type="submit" value="Gửi ngay">
</form>