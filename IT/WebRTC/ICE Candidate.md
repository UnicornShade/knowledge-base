# ICE Candidate
Информация о сетевом соединении и методах коммуникации пиров (напрямую или через [[TURN]]). Обычно каждый пир предлагает от лучших спускаясь до худших кандидатов. В идеале кандидаты UDP, однако [[ICE]] позволяет использовать и TCP

*Не все браузеры поддерживают ICE с TCP*

## UDP кандидаты %%TODO%%
### host
[host кандидат](https://datatracker.ietf.org/doc/html/rfc5245#section-4.1.1.1)
### prflx 
[peer reflexive](https://datatracker.ietf.org/doc/html/rfc5245#section-7.1.3.2.1)
### srflx 
[server reflexive](https://datatracker.ietf.org/doc/html/rfc5245#section-4.1.1.2)
### relay
[relay кандидат](https://datatracker.ietf.org/doc/html/rfc5245#section-4.1.1.2)

## [TCP кандидаты](https://developer.mozilla.org/en-US/docs/Web/API/WebRTC_API/Connectivity#tcp_candidate_types)
### active
### passive
### so