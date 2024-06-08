# sipe-rust-mission-2
## mini grep 만들기

인수의 값 읽을때에는 `std::env::args`를 사용   
하지만, 유니코드가 들어있다면 패닉을 일으킴. 유효하지 않는 유니코드를 받으려면 std::env::args_os를 사용해함.   

```bash
cargo run -- needle haystack
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.00s
    Running `target/debug/sipe-rust-mission-2 needle haystack`
[src/main.rs:7:5] args = [
    "target/debug/sipe-rust-mission-2",
    "needle",
    "haystack",
]
```

벡터의 첫 번째 값이 `"target/debug/sipe-rust-mission-2"`, 즉 이 바이너리 파일의 이름   

