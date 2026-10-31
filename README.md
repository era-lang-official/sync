# Era Sync (`github.com/era-lang-official/sync`)

Concurrency primitives, thread-safe atomic wrappers, FIFO queues, and rate limiters for Era.

## Features
- **AtomicInt**: Load, store, add, sub, and compare-and-swap operations.
- **Queue**: FIFO capacity-bounded queue.
- **RateLimiter**: Token bucket rate limiter for API requests.

## Usage
```era
import "github.com/era-lang-official/sync";

fn main() {
    let mut counter = AtomicInt::new(0);
    counter.add(1);

    let mut q = Queue::new(100);
    q.push("task".to_string());
}
```

