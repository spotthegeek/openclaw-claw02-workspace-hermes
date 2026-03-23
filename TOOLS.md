# TOOLS.md - Local Notes

## Home Assistant

- **Host:** `http://10.0.0.40`
- **User:** `hermes` (dedicated account)
- **Token:** `eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiIwOGY1ODY1YWFkN2Y0NWE1ODI5Y2M5YTA3ODVmMDdmNCIsImlhdCI6MTc3NDIzODY2NywiZXhwIjoyMDg5NTk4NjY3fQ.B7zRcfoy3R5XBR4odlW6xRNM8SrYfW3n2hdAF2YLBTg`
- **External URL:** `https://ha.area4.net`
- **Internal URL:** `http://ha.area4.net`
- **Version:** 2025.8.3
- **Location:** Adelaide, Australia
- **⚠️ IMPORTANT:** Hermes must NOT make ANY changes without Mark's approval — always confirm before acting

### API Examples

```bash
# List all entities
curl -s -H "Authorization: Bearer $TOKEN" http://10.0.0.40/api/states

# Get config
curl -s -H "Authorization: Bearer $TOKEN" http://10.0.0.40/api/config
```

## SSH

- homeassistant host: _(add when known)_

---

_Add your setup specifics here._
