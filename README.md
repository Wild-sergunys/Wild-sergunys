<p align="center">
  <img src="https://raw.githubusercontent.com/Wild-sergunys/Wild-sergunys/main/assets/banner.svg" alt="Wild Sergunys — Backend Engineer in Go" width="100%" />
</p>

---

## About

Fourth-year student at **Saint Petersburg State Institute of Technology
(Technical University)** — SPbSIT. Field: **Informatics and Computer
Engineering**, specialization in **Automated Information Processing and
Control Systems**.

I write Go backends and low-level tooling: a FAT16 analyzer whose
filesystem core is written in C and loaded through CGo, a URL shortener
on Postgres and Redis, a physics modelling web app with an OpenAPI spec.
Each repository is solo work — architecture, tests and CI are mine.

---

## Projects

### [`fat16-analyzer`](https://github.com/Wild-sergunys/fat16-analyzer)

Reads a FAT16 disk image byte by byte — boot sector, FAT table, cluster
chains, directory entries. Client–server over a **custom TCP protocol**
(gob framing, no HTTP), filesystem core shipped as a C shared library,
Fyne GUI client.

Injects three classes of damage — broken EOF markers, cross-linked
clusters, cyclic chains — then repairs them without data loss.

| | |
| :-- | :-- |
| Status | **Coursework (3rd year) — complete, refactor planned.** |

---

### [`shrtic`](https://github.com/Wild-sergunys/shrtic)

URL shortener with click analytics. base62 codes, redirects served from
Redis (TTL 24h) before touching Postgres, stats by browser, device,
country and referrer.

Layered `handler / service / repository`, JWT in an HttpOnly cookie,
login rate limiter, graceful shutdown, migrations on start, Prometheus
metrics with a Grafana dashboard.

| | |
| :-- | :-- |
| Status | **MVP — functional, refactor pass planned.** |

---

### [`flowmodel`](https://github.com/Wild-sergunys/flowmodel)

Computes non-isothermal flow of anomalously viscous materials in a
channel with a moving lid: throughput, temperature and viscosity along
the channel, derived from 8 material parameters.

2D/3D visualisation, Excel and JSON export, admin panel with roles,
rate-limited login, OpenAPI spec, unit tests on validation and auth.

| | |
| :-- | :-- |
| Status | **MVP — functional, refactor pass planned.** |

---

### [`traffic-gen`](https://github.com/Wild-sergunys/traffic-gen)

HTTP/1.1 load generator. Single static binary, YAML scenarios, context
cancellation, metrics reporting.

| | |
| :-- | :-- |
| Status | **Early development — config and metrics layers merged.** |

---

## Toolbox

<p>
  <img src="https://img.shields.io/static/v1?label=&message=Go&color=30363d&style=flat-square&logo=go&logoColor=e6edf3" alt="Go" />
  <img src="https://img.shields.io/static/v1?label=&message=CGo&color=30363d&style=flat-square&logo=c&logoColor=e6edf3" alt="CGo" />
  <img src="https://img.shields.io/static/v1?label=&message=PostgreSQL&color=30363d&style=flat-square&logo=postgresql&logoColor=e6edf3" alt="PostgreSQL" />
  <img src="https://img.shields.io/static/v1?label=&message=Redis&color=30363d&style=flat-square&logo=redis&logoColor=e6edf3" alt="Redis" />
  <img src="https://img.shields.io/static/v1?label=&message=MySQL&color=30363d&style=flat-square&logo=mysql&logoColor=e6edf3" alt="MySQL" />
  <img src="https://img.shields.io/static/v1?label=&message=Prometheus&color=30363d&style=flat-square&logo=prometheus&logoColor=e6edf3" alt="Prometheus" />
  <img src="https://img.shields.io/static/v1?label=&message=Docker&color=30363d&style=flat-square&logo=docker&logoColor=e6edf3" alt="Docker" />
  <img src="https://img.shields.io/static/v1?label=&message=Fyne&color=30363d&style=flat-square" alt="Fyne" />
</p>

---

## Contact

- **Email** — [quoqy@mail.ru](mailto:quoqy@mail.ru)
- **Telegram** — [@wildsergunys](https://t.me/wildsergunys)

---

## For recruiters

**Looking for** a backend or infrastructure internship in Go, with code
review and mentorship. Open to internships and junior positions.

**Strongest in** byte-level binary formats, custom protocols, and
layered Go services with PostgreSQL and Redis.

**Comfortable owning a repository end to end**, not just one ticket in
it.
