# PatientGenius Demo Pages — UMP Practices

Static HTML demos of the Patient Genius Strategic Plays dashboard, customized per UMP-affiliated orthopedic practice. Each folder is self-contained — no shared assets, no cross-navigation.

## Folders

| Folder | Practice | Site |
|---|---|---|
| `aoa/` | AOA Orthopedic Specialists | arlingtonortho.com |
| `abilenesportsmed/` | Abilene Sports Medicine & Orthopedics | abilenesportsmed.com |
| `allstarortho/` | All-Star Orthopaedics | allstarortho.com |
| `ntxortho/` | North Texas Orthopedics & Spine Center | ntxortho.com |
| `orthotexas/` | OrthoTexas | orthotexas.com |
| `orthopedicassociates/` | Orthopedic Associates | orthopedicassociates.org |
| `panoramaortho/` | Panorama Orthopedics & Spine Center | panoramaortho.com |
| `pinnacleortho/` | Pinnacle Orthopaedics | pinnacle-ortho.com |
| `resurgens/` | Resurgens Orthopaedics | resurgens.com |

## Push to GitHub

This folder has a partially-initialized `.git/` from the build environment. Delete it and run a clean init on your machine:

```powershell
# From inside this folder in PowerShell
Remove-Item -Recurse -Force .git
git init -b main
git add .
git commit -m "Initial commit: 9 PatientGenius demo pages for UMP practices"

# Create a new repo on GitHub (private), then:
git remote add origin https://github.com/<your-org>/<repo-name>.git
git push -u origin main
```

## Enable GitHub Pages

In the new repo's Settings → Pages: set Source to `Deploy from a branch`, Branch to `main`, folder to `/ (root)`, and save.

The `.nojekyll` file is already in place to prevent Jekyll processing.

Each demo will then be reachable at distinct URLs:

```
https://<your-org>.github.io/<repo-name>/aoa/
https://<your-org>.github.io/<repo-name>/abilenesportsmed/
https://<your-org>.github.io/<repo-name>/allstarortho/
https://<your-org>.github.io/<repo-name>/ntxortho/
https://<your-org>.github.io/<repo-name>/orthotexas/
https://<your-org>.github.io/<repo-name>/orthopedicassociates/
https://<your-org>.github.io/<repo-name>/panoramaortho/
https://<your-org>.github.io/<repo-name>/pinnacleortho/
https://<your-org>.github.io/<repo-name>/resurgens/
```

No index page or cross-navigation between practices is intended — each URL stands alone.

## Notes

Strategic play numbers (rank shifts, % movements, projected visits, schema entity counts) are illustrative, not measured. The demo banner on each page makes that clear. Practice names, locations, surgeon names, sub-specialty mix, and competitor names are real and verified from public sources as of late April 2026.
