# Digger: Write-up

DNS-сервера хранят о домене не только IP-адрес, на который будет отправляться
запрос при открытии сайта, но и много другой информации, например адреса почтовых
серверов.

Но нас интересует не это: одним из типов записей являются TXT-записи, которые
позволяют "прятать" там произвольную информацию.

Именно этим мы и воспользовались: одна из двух TXT-записей домена `uctf.ml`
содержит флаг.

Догадаться до этого было ещё проще, если вы знали про утилиту `dig` в Linux —
она позволяет узнать DNS-записи домена. В условии было несколько намёков на
необходимость её использования.

Флаг: **uctfyouaregoodatdigging**
