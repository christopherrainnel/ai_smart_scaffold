# Third-Party Notices

**Product:** AI Smart Scaffold
**Version:** 0.1.0
**Date:** 2026-04-01

This file lists the open-source software components used by AI Smart Scaffold and their respective licenses. H&S Nexus Ventures gratefully acknowledges the work of these open-source projects.

---

## Python Runtime Dependencies

| Package | Version | License | Repository |
|---------|---------|---------|------------|
| FastAPI | 0.135.1 | MIT | https://github.com/tiangolo/fastapi |
| Uvicorn | 0.34.0 | BSD-3-Clause | https://github.com/encode/uvicorn |
| Starlette | 0.49.1 | BSD-3-Clause | https://github.com/encode/starlette |
| SQLAlchemy | 2.0.43 | MIT | https://github.com/sqlalchemy/sqlalchemy |
| Pydantic Settings | 2.7.1 | MIT | https://github.com/pydantic/pydantic-settings |
| HTTPX | 0.28.1 | BSD-3-Clause | https://github.com/encode/httpx |
| python-dotenv | 1.0.1 | BSD-3-Clause | https://github.com/theskumar/python-dotenv |
| python-multipart | 0.0.22 | Apache-2.0 | https://github.com/Kludex/python-multipart |
| itsdangerous | 2.2.0 | BSD-3-Clause | https://github.com/pallets/itsdangerous |
| jsonschema | 4.26.0 | MIT | https://github.com/python-jsonschema/jsonschema |

### Transitive Dependencies

The packages above may include transitive dependencies with their own licenses. For a complete list, inspect the installed package metadata using `pip show <package>` or `pip-licenses`.

---

## Development Dependencies

The following are used during development and testing only. They are **not** distributed with the product:

| Package | Version | License | Purpose |
|---------|---------|---------|---------|
| pytest | 8.3.5 | MIT | Test framework |
| ruff | 0.9.10 | MIT | Linter and formatter |
| mypy | 1.15.0 | MIT | Static type checking |
| pip-audit | 2.8.0 | Apache-2.0 | Vulnerability scanning |
| bandit | 1.8.6 | Apache-2.0 | Security linting |
| httpx | 0.27.2 | BSD-3-Clause | Development HTTP client compatibility |
| pytest-asyncio | 0.24.0 | Apache-2.0 | Async test support |
| anyio | 4.6.2 | MIT | Async compatibility during testing |
| pip-tools | 7.5.3 | BSD-3-Clause | Dependency locking |

---

## VS Code Extension Dependencies

The shipped AI Smart Scaffold VS Code extension has no third-party npm runtime dependencies. It uses the VS Code Extension API plus Node.js built-in modules (`node:crypto`, `node:fs`, `node:child_process`).

Extension build and packaging tooling is used during development only and is not distributed as part of the installed extension. This includes TypeScript, Jest, `ts-jest`, type packages, and `@vscode/vsce` when packaging a VSIX.

---

## License Texts

### MIT License

```
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

### BSD 3-Clause License

```
Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice,
   this list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its contributors
   may be used to endorse or promote products derived from this software
   without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Apache License 2.0

```
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

---

## Keeping This File Current

When runtime or development dependencies change (additions, removals, or version bumps in `requirements.in` or `requirements-dev.txt`), this file must be regenerated to reflect the current release snapshot. This step is included in the product release checklist.


