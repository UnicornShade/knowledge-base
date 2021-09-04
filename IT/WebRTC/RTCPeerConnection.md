Для установки соединения между локальным компьютером и удаленным пиром.  При открытии соединения в него могут добавляться [[MediaStream]] или [[RTCDataChannel]].

Наследуется от EventTarget

Предоставляет методы для соединения к удаленному пиру, поддержки и мониторингу соединения и закрытия соединения

## Properties
### `canTrickleIceCandidates` 
_readonly_  [[ICE]] candidate
### `connectionState`
_readonly_ [[RTCPeerConnectionState]]
### `currentLocalDescription`
_readonly_ локальный [[RTCSessionDescription]], уже находящися в стейте [[SessionDescription#Local description]]
### `currentRemoteDescription`
_readonly_ ремоут [[RTCSessionDescription]] ⬆️ [[SessionDescription#Remote description]]
### `iceConnectionState`
_readonly_ [[IceConnectionState]] [[ICE]] candidate
### `iceGatheringState`
_readonly_ [[IceGatheringState]]
### `localDescription`
_readonly_ [[RTCSessionDescription]] Возвращает [[#pendingLocalDescription]] ?? [[#currentLocalDescription]]
### `peerIdentity`
_readonly_ [[RTCIdentityAssertion]] айдишник ремоут пира. Как только промис резолвится айдишник не меняется все соединение
### `pendingLocalDescription`
_readonly_ отражает не текущее состояние [[RTCSessionDescription]], а его ближайшее будущее
### `pendingRemoteDescription`
_readonly_ ремоут [[RTCSessionDescription]] ⬆️
### `remoteDescription`
_readonly_ аналогично [[#localDescription]]
### `sctp`
_readonly_ [[RTCSctpTransport]] объект с характеристиками  [[SCTP]] транспортного уровня
### `signalingState`
_readonly_ состояние процесса [[Signaling]] может быть [[SignalingState]]

## Methods
### `addIceCandidate`
### `addTrack`
### `addTransceiver`
### `close`
### `createAnswer`
### `createDataChannel`
### `createOffer`
### `getConfiguration`
### `getIndentityAssertion`
### `getReceivers`
### `getSenders`
### `getStats`
### `getTransceivers`
### `removeTrack`
### `restartIce`
### `setConfiguration`
### `setIdentityProvider`
### `setLocalDescription`
### `setRemoteDescription`

## Event handlers
`onconnectionstatechange` 
`ondatachannel`
`onicecandidate`
`onicecandidateerror`
`oniceconnectionstatechange`
`onicegatheringstatechange`
`onnegotationneeded`
`onsignalingstatechange`
`ontrack`
