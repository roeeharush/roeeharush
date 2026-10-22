# 👋 Hi, I'm Roee

**3rd-year Software Engineering student at SCE (Shamoon College of Engineering)**, looking for my first
student software developer position.

I like understanding how systems work and measuring them, not just making them run.

<p>
  <img src="https://skillicons.dev/icons?i=cpp,java,py,linux,git,github&theme=dark" alt="C++, Java, Python, Linux, Git, GitHub" />
</p>

---

## 🚀 Projects

### 🛰️ [SentinelRT](https://github.com/roeeharush/sentinel-rt) &nbsp;`C++17`

A simulation and monitoring platform. Simulated devices send sensor measurements over TCP to a
multithreaded server that detects threshold violations, stuck and drifting sensors, and device timeouts.

- 🧵 **Concurrency:** a bounded producer-consumer queue with backpressure, and a worker thread pool.
- 🌐 **Networking:** TCP with length-prefixed message framing.
- 🧪 **Quality:** a test suite of unit tests and deterministic scenarios, clean under AddressSanitizer,
  UndefinedBehaviorSanitizer and ThreadSanitizer.
- 📊 **Measured performance:** a benchmark program and a Python automation script. The README documents the
  method, the results and the limitations.

**A finding from the measurements:** waking a blocked producer on every dequeue limited throughput.
Changing the wake-up policy fixed it.

| 2 worker threads, saturated queue | Throughput |
|---|---|
| Before the change | about 141,000 items/s |
| After the change | about 2,370,000 items/s |

*(One machine, Ubuntu on WSL2, median of 3 runs. Details and caveats are in the project's README.)*

### 🌿 [The Reserve](https://github.com/roeeharush/TheReserve) &nbsp;`Java`

A multithreaded, network-enabled ecosystem simulation with a Swing GUI, built together with a project
partner. We worked in pairs and reviewed each other's changes.

- 🧵 Each entity runs on its own thread and requests actions through a blocking command queue, so changes
  to the model stay single-writer.
- 🌐 A TCP server lets an external client spawn entities.
- 🧩 Uses the Strategy, State, Command, Decorator, Factory Method, Observer and MVC patterns.

---

## 🛠️ Tech

| | |
|---|---|
| **Languages** | C++17, Java, Python |
| **Systems** | Linux (WSL2), TCP/IP sockets, multithreading |
| **Practices** | Unit and scenario testing, sanitizers (ASan, UBSan, TSan), benchmarking, design patterns, Git |

## 🎓 Education

B.Sc. in Computer Software Engineering, SCE - Shamoon College of Engineering (2025 - 2028).
🏅 Department Excellence Award, Year 1.

## 🔎 What I'm looking for

My first student software developer position: a place where I can contribute, learn from experienced
mentors and grow with the team.

## 📫 Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Roee_Harush-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/roee-harush-software-engineer/)
