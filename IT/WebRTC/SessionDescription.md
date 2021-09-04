# Session Description
Конфигурация эндпоинта WebRTC соединения

При старте звонка другому юзеру создается session description **offer**. Получатель отвечает **answer**. Оба устройства обмениваются информацией для возможности обмена медиа данными. Обмен производится с использованием [[ICE]] протокола

Каждый пир получает два description: local и remote. 


## Local description
Описывает себя

## Remote description
Описывает удаленный пир

## Current description
[[RTCPeerConnection#currentLocalDescription]] [[RTCPeerConnection#currentRemoteDescription]] описывает текущий description, используемый в соединении. Последнее соединение, о котором полностью договорились оба пира

## Pending description
[[RTCPeerConnection#pendingLocalDescription]] [[RTCPeerConnection#pendingRemoteDescription]] description, который рассматривается пирами


[[SDP]]