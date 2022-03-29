# Virtual Machines / Virtual OS: Summary

### Pro

- Separated environments
- Environment-specific configurations are possible
- Environment configurations can be shared and reproduced reliably

### Con

- Redundant duplication, waste of space
- Performance can be slow, boot times can be long
- Reproducing on another computer / server is possible but may still be tricky

# Containers vs Virtual Machines

### Docker Containers

- Low impact on OS, very fast, minimal disk space usage
- Sharing, re-building and distribution is easy
- Encapsulate apps / environments instead of "whole machines"

### Virtual Machines

- Bigger impact on OS, slower, higher disk space usage
- Sharing, re-building and distribution can be challenging
- Encapsulate "whole machines" instead of just apps / environments
