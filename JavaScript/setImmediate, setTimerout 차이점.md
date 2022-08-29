## setImmediate(콜백)과 setTimeout(콜백, 0) 차이점
setImmediate(콜백)과 setTimeout(콜백, 0)에 담긴 콜백 함수는 이벤트 루프를 거친 뒤 즉시 실행됩니다. 둘의 차이점은 setImmediate는 setTimeout(콜백, 0)보다 먼저 실행됩니다.
파일 시스템 접근, 네트워킹 같은 I/O 작업의 콜백 함수 안에서 타이머를 호출하는 경우입니다. setImmediate가 항상 setTimeout(콜백, 0)보다 먼저 호출되지는 않는다는 점입니다.
setTimeout(콜백, 0)은 사용하지 않는 것을 권장합니다.
