# macbook_settings

macOS Sierra에서 업데이트 후 키보드 한글 입력 상태에서는 백 쿼트(`) 키를 누르면 원화(₩)가 입력된다.
한글 입력 상태에서는 옵션키와 함께 백 쿼트(`)키를 눌러야 백 쿼트(`)를 입력 할 수 있다.
마크다운 문서를 작성하는 사람이나 개발자에게는 매우 불편하다.

# 해결 방법
```
~/Library 폴더로 이동해서 KeyBindings 폴더를 추가한다.
~/Library/KeyBindings 폴더에 DefaultkeyBinding.dict 파일을 만든다.
DefaultkeyBinding.dict 파일에 아래의 코드를 추가한다.
{
    "₩" = ("insertText:", "`");
}
```
