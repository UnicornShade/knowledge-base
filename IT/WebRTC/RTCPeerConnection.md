Для установки соединения между локальным компьютером и удаленным пиром.  При открытии соединения в него могут добавляться [[MediaStream]] или [[RTCDataChannel]].

Наследуется от EventTarget

Предоставляет методы для соединения к удаленному пиру, поддержки и мониторингу соединения и закрытия соединения

## Properties
readonly `canTrickleIceCandidates`  [[ICE]] candidate
readonly `connectionState` [[RTCPeerConnectionState]]
readonly `currentLocalDescription` локальный [[RTCSessionDescription]], уже находящися в стейте [[SessionDescription#Local description]]
readonly `currentRemoteDescription` ремоут [[RTCSessionDescription]] ⬆️ [[SessionDescription#Remote description]]
readonly `iceConnectionState` [[IceConnectionState]] [[ICE]] candidate
readonly `iceGatheringState` [[IceGatheringState]]
readonly `localDescription` [[RTCSessionDescription]] Возвращает `pendingLocalDescription ?? currentLocalDescription`
readonly `peerIdentity` [[RTCIdentityAssertion]] айдишник ремоут пира. Как только промис резолвится айдишник не меняется все соединение
readonly `pendingLocalDescription` отражает не текущее состояние [[RTCSessionDescription]], а его ближайшее будущее
readonly `pendingRemoteDescription` ремоут [[RTCSessionDescription]] ⬆️
readonly `remoteDescription` аналогично localDescription [[RTCSessionDescription]]
readonly `sctp` [[RTCSctpTransport]] объект с характеристиками  [[SCTP]] транспортного уровня
readonly `signalingState` состояние процесса [[Signaling]] может быть [[SignalingState]]

## Methods
`addIceCandidate`
`addTrack`
`addTransceiver`
`close`
`createAnswer`
`createDataChannel`
`createOffer`
`getConfiguration`
`getIndentityAssertion`
`getReceivers`
`getSenders`
`getStats`
`getTransceivers`
`removeTrack`
`restartIce`
`setConfiguration`
`setIdentityProvider`
`setLocalDescription`
`setRemoteDescription`

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
