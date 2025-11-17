Here you go, Abhi — **clean, professional, copy-ready block** with:

✅ Copy button–friendly formatting
✅ `echo` statements for **COMPANY** and **PROJECT**
✅ Zero repetition
✅ Same variable structure you use everywhere

---

# ✅ **FINAL COPY-READY GLOBAL VARIABLES (with echo)**

```bash
# ---------------------------
# GLOBAL (APPLIES TO ALL ENVS)
# ---------------------------

# Auto-fetch Tenant + Subscription
export TENANT_ID=$(az account show --query tenantId -o tsv)
export SUBSCRIPTION_ID=$(az account show --query id -o tsv)

# Company / Project
export COMPANY="fintrust"
export PROJECT="simplecrud"

# Echo confirmation
echo "✅ COMPANY set to: $COMPANY"
echo "✅ PROJECT set to: $PROJECT"

# CAF Regions
export PRIMARY_LOCATION="eastus"
export PRIMARY_LOCATION_SHORT="eus"
export DR_LOCATION="westus"
export DR_LOCATION_SHORT="wus"

# Common Tags
export TAG_OWNER="Abhi"
export TAG_COST_CENTER="FinTrust-Training"
export TAG_PROJECT="${PROJECT}"

# CAF Management Groups
export MG_ROOT="${COMPANY}-root"
export MG_PLATFORM="${COMPANY}-platform"
export MG_CONNECTIVITY="${COMPANY}-connectivity"
export MG_IDENTITY="${COMPANY}-identity"
export MG_LZ_APP="${COMPANY}-lz-app"
export MG_LZ_DATA="${COMPANY}-lz-data"


echo "📌 Primary:       $PRIMARY_LOCATION ($PRIMARY_LOCATION_SHORT)"
echo "📌 DR:            $DR_LOCATION ($DR_LOCATION_SHORT)"
```

---

### Want a version with full **color output** or **emoji indicators** (success/failure) using `tput`?
