---
description: "TypeScript Node Configuration (tsconfig.node.json)"
globs: "**/*"
---

rule TypeScriptNodeConfig
description "Ensure TypeScript node configuration supports strict mode, ESNext, and synthetic imports."
config-file "tsconfig.node.json"
config-content """
{
  "compilerOptions": {
    "composite": true,
    "tsBuildInfoFile": "./node_modules/.tmp/tsconfig.node.tsbuildinfo",
    "skipLibCheck": true,
    "module": "ESNext",
    "moduleResolution": "bundler",
    "allowSyntheticDefaultImports": true,
    "strict": true,
    "noEmit": true
  },
  "include": ["vite.config.ts"]
}
"""