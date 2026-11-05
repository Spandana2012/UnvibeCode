# UnvibeCode — Flask Analysis Project

This repository packages a reproducible UnvibeCode analysis of the
[Flask](https://flask.palletsprojects.com/) framework, together with the
analyzed Flask source snapshot and the generated review artifacts.

## Contents

| Path | Purpose |
| --- | --- |
| `flask/` | Flask source snapshot analyzed by UnvibeCode. |
| `unvibecode_results/flask-unvibecode-analysis-20261105_115520/` | Complete analysis output, reports, and technical logs. |
| `unvibecode_results/.../flask-unvibecode-full.html` | Main self-contained analysis report. |
| `unvibecode_results/.../report-support/` | Business workflow, connected-code, and risk-finding report sections. |

## View the results

Open `unvibecode_results/flask-unvibecode-analysis-20261105_115520/flask-unvibecode-full.html`
in a web browser. It is the primary, self-contained report.

The `technical-logs/` folder retains the workflow and code-mapping logs for
traceability. `flask-repository-context.zip` is the source-context archive
produced with the analysis.

## Work with the Flask source

The source snapshot declares Python 3.11 or later. From the `flask` directory:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -U pip
python -m pip install -e ".[tests]"
pytest
```

For the full upstream documentation and contributor guidance, see
[`flask/README.md`](flask/README.md) and [`flask/LICENSE.txt`](flask/LICENSE.txt).

## Provenance

The analyzed source is Flask, originally from the
[Pallets Flask repository](https://github.com/pallets/flask), at snapshot
commit `49943b5a`. Flask is distributed under the BSD 3-Clause License; its
license is retained in `flask/LICENSE.txt`.

## License

The analysis artifacts in this repository are provided by the repository
owner. The `flask/` directory remains subject to Flask's BSD 3-Clause License.
