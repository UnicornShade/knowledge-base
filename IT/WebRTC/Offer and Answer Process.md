## Установка соединения между двумя пирами
1. Звонящий захватывает медиапотоки через getUserMedia
2. Звонящий создает [[RTCPeerConnection]] и вызывает [[RTCPeerConnection#addTrack]]
3. Звонящий создает оффер через [[RTCPeerConnection#createOffer]]
4. Звонящий кладет оффер в [[SessionDescription#Local description]] через [[RTCPeerConnection#setLocalDescription]]
5. После установки local description звонящий просит [[STUN]] сервер сгенерировать [[ICE Candidate]]
6. Звонящий использует [[Signaling]] сервер для передачи оффера вызываемому абоненту
7. Вызываемый получает оффер и вызывает [[RTCPeerConnection#setRemoteDescription]] для записи [[SessionDescription#Remote description]]
8. Вызываемый проводит подготовку для его стороны звонка захватывает локальные медиа и добавляет их в соединение через [[RTCPeerConnection#addTrack]]
9. Вызываемый созает ответ через вызов [[RTCPeerConnection#createAnswer]]
10. Вызываемый дергает [[RTCPeerConnection#setLocalDescription]], чтобы установить ответ в [[SessionDescription#Local description]]. Вызываемый знает оба конца конфигурации соединения
11. Вызываемый использует [[Signaling]] сервер для отправки ответа звонящему
12. Звонящий получает ответ
13. Звонящий вызывает [[RTCPeerConnection#setRemoteDescription]] для установки ответа в [[SessionDescription#Remote description]]. Звонящий знает оба конца конфигурации соединения. Медиа потоки передаются как сконфигурированы

## Pending and current descriptions
[[SessionDescription#Current Description]] [[SessionDescription#Pending description]]
Во время [[Renegotiation]] оффер может быть отклонен изза предложения неправильного формата. Для этого используются текущее и предстоящее [[SessionDescription]]