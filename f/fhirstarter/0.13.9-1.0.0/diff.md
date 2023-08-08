# Comparing `tmp/fhirstarter-0.13.9.tar.gz` & `tmp/fhirstarter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhirstarter-0.13.9.tar", max compression
+gzip compressed data, was "fhirstarter-1.0.0.tar", max compression
```

## Comparing `fhirstarter-0.13.9.tar` & `fhirstarter-1.0.0.tar`

### file list

```diff
@@ -1,173 +1,50 @@
--rw-r--r--   0        0        0     1071 2023-01-25 15:18:03.969523 fhirstarter-0.13.9/LICENSE.md
--rw-r--r--   0        0        0     6076 2023-01-25 16:41:17.839630 fhirstarter-0.13.9/README.md
--rw-r--r--   0        0        0      388 2023-07-28 02:58:19.651849 fhirstarter-0.13.9/fhirstarter/__init__.py
--rw-r--r--   0        0        0     3928 2023-08-01 20:37:57.327357 fhirstarter-0.13.9/fhirstarter/exceptions.py
--rw-r--r--   0        0        0      148 2022-09-02 16:13:21.196164 fhirstarter-0.13.9/fhirstarter/fhir_specification/__init__.py
--rw-r--r--   0        0        0     1216 2022-08-30 15:52:43.914830 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/account-example.json
--rw-r--r--   0        0        0     9898 2022-08-30 15:52:43.919849 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/activitydefinition-example.json
--rw-r--r--   0        0        0     3652 2022-08-30 15:52:43.924678 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/adverseevent-example.json
--rw-r--r--   0        0        0     6761 2022-08-30 15:52:43.930277 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/allergyintolerance-example.json
--rw-r--r--   0        0        0     2477 2022-08-30 15:52:43.937169 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/appointment-example.json
--rw-r--r--   0        0        0      654 2022-08-30 15:52:43.943319 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/appointmentresponse-example.json
--rw-r--r--   0        0        0     3080 2022-08-30 15:52:43.949392 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/auditevent-example.json
--rw-r--r--   0        0        0     2587 2022-08-30 15:52:43.955039 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/basic-example.json
--rw-r--r--   0        0        0   176064 2022-08-30 15:52:43.966340 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/binary-example.json
--rw-r--r--   0        0        0      409 2022-08-30 15:52:43.972693 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/biologicallyderivedproduct-example.json
--rw-r--r--   0        0        0     1459 2022-08-30 15:52:43.978291 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/bodystructure-example.json
--rw-r--r--   0        0        0     2364 2022-08-30 15:52:43.984348 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/bundle-example.json
--rw-r--r--   0        0        0     5930 2022-08-30 15:52:43.991165 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/capabilitystatement-example.json
--rw-r--r--   0        0        0     3597 2022-08-30 15:52:43.996869 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/careplan-example.json
--rw-r--r--   0        0        0     1767 2022-08-30 15:52:44.002022 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/careteam-example.json
--rw-r--r--   0        0        0      624 2022-08-30 15:52:44.008313 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/catalogentry-example.json
--rw-r--r--   0        0        0     2862 2022-08-30 15:52:44.014027 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/chargeitem-example.json
--rw-r--r--   0        0        0     3418 2022-08-30 15:52:44.019871 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/chargeitemdefinition-example.json
--rw-r--r--   0        0        0     2057 2022-08-30 15:52:44.025691 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/claim-example.json
--rw-r--r--   0        0        0     3631 2022-08-30 15:52:44.030893 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/claimresponse-example.json
--rw-r--r--   0        0        0     3774 2022-08-30 15:52:44.036000 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/clinicalimpression-example.json
--rw-r--r--   0        0        0     3970 2022-08-30 15:52:44.041990 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/codesystem-example.json
--rw-r--r--   0        0        0     1729 2022-08-30 15:52:44.047864 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/communication-example.json
--rw-r--r--   0        0        0      551 2022-08-30 15:52:44.052717 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/communicationrequest-example.json
--rw-r--r--   0        0        0     3674 2022-08-30 15:52:44.057949 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/compartmentdefinition-example.json
--rw-r--r--   0        0        0     5631 2022-08-30 15:52:44.062736 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/composition-example.json
--rw-r--r--   0        0        0     5377 2022-08-30 15:52:44.067640 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/conceptmap-example.json
--rw-r--r--   0        0        0     1798 2022-08-30 15:52:44.072541 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/condition-example.json
--rw-r--r--   0        0        0     1552 2022-08-30 15:52:44.077542 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/consent-example.json
--rw-r--r--   0        0        0     2085 2022-08-30 15:52:44.082554 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/contract-example.json
--rw-r--r--   0        0        0     4163 2022-08-30 15:52:44.087552 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/coverage-example.json
--rw-r--r--   0        0        0     1027 2022-08-30 15:52:44.092546 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/coverageeligibilityrequest-example.json
--rw-r--r--   0        0        0     1090 2022-08-30 15:52:44.098557 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/coverageeligibilityresponse-example.json
--rw-r--r--   0        0        0     2834 2022-08-30 15:52:44.103606 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/detectedissue-example.json
--rw-r--r--   0        0        0      701 2022-08-30 15:52:44.108516 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/device-example.json
--rw-r--r--   0        0        0      651 2022-08-30 15:52:44.113536 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/devicedefinition-example.json
--rw-r--r--   0        0        0     2998 2022-08-30 15:52:44.118529 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/devicemetric-example.json
--rw-r--r--   0        0        0     1050 2022-08-30 15:52:44.123489 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/devicerequest-example.json
--rw-r--r--   0        0        0     1422 2022-08-30 15:52:44.129521 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/deviceusestatement-example.json
--rw-r--r--   0        0        0     6944 2022-08-30 15:52:44.134490 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/diagnosticreport-example.json
--rw-r--r--   0        0        0     1640 2022-08-30 15:52:44.139915 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/documentmanifest-example.json
--rw-r--r--   0        0        0     8433 2022-08-30 15:52:44.144723 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/documentreference-example.json
--rw-r--r--   0        0        0      699 2022-08-30 15:52:44.149530 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/effectevidencesynthesis-example.json
--rw-r--r--   0        0        0      625 2022-08-30 15:52:44.154502 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/encounter-example.json
--rw-r--r--   0        0        0     1388 2022-08-30 15:52:44.159630 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/endpoint-example.json
--rw-r--r--   0        0        0      815 2022-08-30 15:52:44.164543 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/enrollmentrequest-example.json
--rw-r--r--   0        0        0      899 2022-08-30 15:52:44.169570 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/enrollmentresponse-example.json
--rw-r--r--   0        0        0     2332 2022-08-30 15:52:44.174554 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/episodeofcare-example.json
--rw-r--r--   0        0        0      991 2022-08-30 15:52:44.179542 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/eventdefinition-example.json
--rw-r--r--   0        0        0      487 2022-08-30 15:52:44.185247 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/evidence-example.json
--rw-r--r--   0        0        0      548 2022-08-30 15:52:44.190874 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/evidencevariable-example.json
--rw-r--r--   0        0        0    29430 2022-08-30 15:52:44.196200 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/examplescenario-example.json
--rw-r--r--   0        0        0     6629 2022-08-30 15:52:44.202041 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/explanationofbenefit-example.json
--rw-r--r--   0        0        0     1630 2022-08-30 15:52:44.207655 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/familymemberhistory-example.json
--rw-r--r--   0        0        0     1245 2022-08-30 15:52:44.212638 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/flag-example.json
--rw-r--r--   0        0        0     2154 2022-08-30 15:52:44.217647 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/goal-example.json
--rw-r--r--   0        0        0     3485 2022-08-30 15:52:44.222517 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/graphdefinition-example.json
--rw-r--r--   0        0        0     1113 2022-08-30 15:52:44.227445 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/group-example.json
--rw-r--r--   0        0        0     3182 2022-08-30 15:52:44.232442 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/guidanceresponse-example.json
--rw-r--r--   0        0        0     4747 2022-08-30 15:52:44.237476 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/healthcareservice-example.json
--rw-r--r--   0        0        0     1523 2022-08-30 15:52:44.242623 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/imagingstudy-example.json
--rw-r--r--   0        0        0     7176 2022-08-30 15:52:44.247964 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/immunization-example.json
--rw-r--r--   0        0        0     2620 2022-08-30 15:52:44.253554 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/immunizationevaluation-example.json
--rw-r--r--   0        0        0     2536 2022-08-30 15:52:44.258792 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/immunizationrecommendation-example.json
--rw-r--r--   0        0        0     9120 2022-08-30 15:52:44.263610 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/implementationguide-example.json
--rw-r--r--   0        0        0      607 2022-08-30 15:52:44.269048 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/insuranceplan-example.json
--rw-r--r--   0        0        0     1239 2022-08-30 15:52:44.274503 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/invoice-example.json
--rw-r--r--   0        0        0     9390 2022-08-30 15:52:44.280642 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/library-example.json
--rw-r--r--   0        0        0     1138 2022-08-30 15:52:44.286280 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/linkage-example.json
--rw-r--r--   0        0        0     2129 2022-08-30 15:52:44.291599 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/list-example.json
--rw-r--r--   0        0        0     1699 2022-08-30 15:52:44.296717 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/location-example.json
--rw-r--r--   0        0        0    16513 2022-08-30 15:52:44.301745 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/measure-example.json
--rw-r--r--   0        0        0    64009 2022-08-30 15:52:44.306667 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/measurereport-example.json
--rw-r--r--   0        0        0     6590 2022-08-30 15:52:44.312958 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/media-example.json
--rw-r--r--   0        0        0     2142 2022-08-30 15:52:44.318502 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medication-example.json
--rw-r--r--   0        0        0     4533 2022-08-30 15:52:44.324461 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicationadministration-example.json
--rw-r--r--   0        0        0     4184 2022-08-30 15:52:44.329434 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicationdispense-example.json
--rw-r--r--   0        0        0     2310 2022-08-30 15:52:44.334475 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicationknowledge-example.json
--rw-r--r--   0        0        0     6390 2022-08-30 15:52:44.339470 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicationrequest-example.json
--rw-r--r--   0        0        0     5865 2022-08-30 15:52:44.344399 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicationstatement-example.json
--rw-r--r--   0        0        0     6646 2022-08-30 15:52:44.349460 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproduct-example.json
--rw-r--r--   0        0        0     5755 2022-08-30 15:52:44.354417 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductauthorization-example.json
--rw-r--r--   0        0        0     1690 2022-08-30 15:52:44.359366 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductcontraindication-example.json
--rw-r--r--   0        0        0     3236 2022-08-30 15:52:44.364408 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductindication-example.json
--rw-r--r--   0        0        0     3181 2022-08-30 15:52:44.369343 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductingredient-example.json
--rw-r--r--   0        0        0     5478 2022-08-30 15:52:44.374667 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductinteraction-example.json
--rw-r--r--   0        0        0     2096 2022-08-30 15:52:44.379989 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductmanufactured-example.json
--rw-r--r--   0        0        0     5966 2022-08-30 15:52:44.385555 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductpackaged-example.json
--rw-r--r--   0        0        0     2454 2022-08-30 15:52:44.390624 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductpharmaceutical-example.json
--rw-r--r--   0        0        0     2137 2022-08-30 15:52:44.395562 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/medicinalproductundesirableeffect-example.json
--rw-r--r--   0        0        0      824 2022-08-30 15:52:44.401466 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/messagedefinition-example.json
--rw-r--r--   0        0        0     1755 2022-08-30 15:52:44.407690 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/messageheader-example.json
--rw-r--r--   0        0        0     3547 2022-08-30 15:52:44.413801 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/molecularsequence-example.json
--rw-r--r--   0        0        0     1894 2022-08-30 15:52:44.419611 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/namingsystem-example.json
--rw-r--r--   0        0        0     3554 2022-08-30 15:52:44.424809 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/nutritionorder-example.json
--rw-r--r--   0        0        0     2949 2022-11-07 16:57:04.761702 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/observation-example.json
--rw-r--r--   0        0        0      982 2022-08-30 15:52:44.436677 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/observationdefinition-example.json
--rw-r--r--   0        0        0     7234 2022-08-30 15:52:44.441379 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/operationdefinition-example.json
--rw-r--r--   0        0        0      880 2022-08-30 15:52:44.446343 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/operationoutcome-example.json
--rw-r--r--   0        0        0     1397 2022-08-30 15:52:44.451403 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/organization-example.json
--rw-r--r--   0        0        0     1748 2022-08-30 15:52:44.456447 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/organizationaffiliation-example.json
--rw-r--r--   0        0        0      847 2022-08-30 15:52:44.461895 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/parameters-example.json
--rw-r--r--   0        0        0     4270 2022-08-30 15:52:44.467481 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/patient-example.json
--rw-r--r--   0        0        0     1296 2022-08-30 15:52:44.472966 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/paymentnotice-example.json
--rw-r--r--   0        0        0     3381 2022-08-30 15:52:44.478703 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/paymentreconciliation-example.json
--rw-r--r--   0        0        0     2610 2022-08-30 15:52:44.483604 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/person-example.json
--rw-r--r--   0        0        0    53475 2022-08-30 15:52:44.488802 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/plandefinition-example.json
--rw-r--r--   0        0        0     1522 2022-08-30 15:52:44.494902 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/practitioner-example.json
--rw-r--r--   0        0        0     2403 2022-08-30 15:52:44.500378 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/practitionerrole-example.json
--rw-r--r--   0        0        0     1367 2022-08-30 15:52:44.505730 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/procedure-example.json
--rw-r--r--   0        0        0     1791 2022-08-30 15:52:44.511380 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/provenance-example.json
--rw-r--r--   0        0        0     5008 2022-08-30 15:52:44.516677 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/questionnaire-example.json
--rw-r--r--   0        0        0     3983 2022-08-30 15:52:44.521671 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/questionnaireresponse-example.json
--rw-r--r--   0        0        0     2265 2022-08-30 15:52:44.527161 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/relatedperson-example.json
--rw-r--r--   0        0        0     3201 2022-08-30 15:52:44.533564 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/requestgroup-example.json
--rw-r--r--   0        0        0      498 2022-08-30 15:52:44.538791 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/researchdefinition-example.json
--rw-r--r--   0        0        0      581 2022-08-30 15:52:44.544528 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/researchelementdefinition-example.json
--rw-r--r--   0        0        0      421 2022-08-30 15:52:44.549419 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/researchstudy-example.json
--rw-r--r--   0        0        0      704 2022-08-30 15:52:44.554478 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/researchsubject-example.json
--rw-r--r--   0        0        0     5755 2022-08-30 15:52:44.560988 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/riskassessment-example.json
--rw-r--r--   0        0        0      556 2022-08-30 15:52:44.566676 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/riskevidencesynthesis-example.json
--rw-r--r--   0        0        0     1369 2022-08-30 15:52:44.571722 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/schedule-example.json
--rw-r--r--   0        0        0     3814 2022-08-30 15:52:44.577444 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/searchparameter-example.json
--rw-r--r--   0        0        0      917 2022-08-30 15:52:44.582378 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/servicerequest-example.json
--rw-r--r--   0        0        0     1358 2022-08-30 15:52:44.587344 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/slot-example.json
--rw-r--r--   0        0        0     5623 2022-08-30 15:52:44.592354 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/specimen-example.json
--rw-r--r--   0        0        0     9978 2022-08-30 15:52:44.597498 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/specimendefinition-example.json
--rw-r--r--   0        0        0   214410 2022-08-30 15:52:44.604373 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/structureddefinition-example.json
--rw-r--r--   0        0        0     4902 2022-08-30 15:52:44.614542 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/structuremap-example.json
--rw-r--r--   0        0        0      880 2022-08-30 15:52:44.628318 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/subscription-example.json
--rw-r--r--   0        0        0     1468 2022-08-30 15:52:44.633460 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substance-example.json
--rw-r--r--   0        0        0      536 2022-08-30 15:52:44.638798 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substancenucleicacid-example.json
--rw-r--r--   0        0        0      536 2022-08-30 15:52:44.639220 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substancepolymer-example.json
--rw-r--r--   0        0        0      536 2022-08-30 15:52:44.639533 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substanceprotein-example.json
--rw-r--r--   0        0        0      536 2022-08-30 15:52:44.639838 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substancereferenceinformation-example.json
--rw-r--r--   0        0        0      253 2022-08-30 15:52:44.645463 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substancesourcematerial-example.json
--rw-r--r--   0        0        0      536 2022-08-30 15:52:44.645807 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/substancespecification-example.json
--rw-r--r--   0        0        0     2730 2022-08-30 15:52:44.651360 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/supplydelivery-example.json
--rw-r--r--   0        0        0     1933 2022-08-30 15:52:44.656258 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/supplyrequest-example.json
--rw-r--r--   0        0        0     5629 2022-08-30 15:52:44.661239 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/task-example.json
--rw-r--r--   0        0        0     1572 2022-08-30 15:52:44.667194 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/terminologycapabilities-example.json
--rw-r--r--   0        0        0    12159 2022-08-30 15:52:44.672226 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/testreport-example.json
--rw-r--r--   0        0        0    26297 2022-08-30 15:52:44.677517 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/testscript-example.json
--rw-r--r--   0        0        0     3483 2022-08-30 15:52:44.682322 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/valueset-example.json
--rw-r--r--   0        0        0      626 2022-08-30 15:52:44.687186 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/verificationresult-example.json
--rw-r--r--   0        0        0     1675 2022-08-30 15:52:44.692236 fhirstarter-0.13.9/fhirstarter/fhir_specification/examples/visionprescription-example.json
--rw-r--r--   0        0        0  2143339 2022-08-30 15:52:44.696052 fhirstarter-0.13.9/fhirstarter/fhir_specification/search-parameters.json
--rw-r--r--   0        0        0     5484 2023-04-17 15:18:28.275081 fhirstarter-0.13.9/fhirstarter/fhir_specification/utils.py
--rw-r--r--   0        0        0    26608 2023-08-01 20:37:57.329562 fhirstarter-0.13.9/fhirstarter/fhirstarter.py
--rw-r--r--   0        0        0    10222 2023-01-24 20:53:50.967128 fhirstarter-0.13.9/fhirstarter/functions.py
--rw-r--r--   0        0        0     3462 2022-08-16 17:25:05.513384 fhirstarter-0.13.9/fhirstarter/interactions.py
--rw-r--r--   0        0        0     4555 2022-08-16 17:25:05.518559 fhirstarter-0.13.9/fhirstarter/providers.py
--rw-r--r--   0        0        0      151 2023-04-17 15:15:02.746821 fhirstarter-0.13.9/fhirstarter/scripts/config.toml
--rw-r--r--   0        0        0     3991 2023-07-31 15:56:50.467585 fhirstarter-0.13.9/fhirstarter/scripts/example.py
--rw-r--r--   0        0        0     8419 2023-08-01 20:37:57.352997 fhirstarter-0.13.9/fhirstarter/search_parameters.py
--rw-r--r--   0        0        0       68 2022-06-21 20:10:12.695171 fhirstarter-0.13.9/fhirstarter/testclient.py
--rw-r--r--   0        0        0        0 2022-08-30 15:52:44.718623 fhirstarter-0.13.9/fhirstarter/tests/__init__.py
--rw-r--r--   0        0        0     3332 2023-07-31 14:50:49.081727 fhirstarter-0.13.9/fhirstarter/tests/config.py
--rw-r--r--   0        0        0      814 2023-07-31 14:50:49.054804 fhirstarter-0.13.9/fhirstarter/tests/conftest.py
--rw-r--r--   0        0        0     6049 2023-07-31 14:50:49.077560 fhirstarter-0.13.9/fhirstarter/tests/test_capability_statement.py
--rw-r--r--   0        0        0     2435 2023-07-31 14:50:49.085971 fhirstarter-0.13.9/fhirstarter/tests/test_dependencies.py
--rw-r--r--   0        0        0     5531 2023-07-31 14:50:49.091215 fhirstarter-0.13.9/fhirstarter/tests/test_errors.py
--rw-r--r--   0        0        0    10467 2023-07-31 14:50:49.060925 fhirstarter-0.13.9/fhirstarter/tests/test_interactions.py
--rw-r--r--   0        0        0     5315 2023-08-01 20:37:57.356357 fhirstarter-0.13.9/fhirstarter/tests/test_utils.py
--rw-r--r--   0        0        0     2363 2023-08-01 20:37:57.359406 fhirstarter-0.13.9/fhirstarter/tests/utils.py
--rw-r--r--   0        0        0    17019 2023-08-01 20:37:57.363539 fhirstarter-0.13.9/fhirstarter/utils.py
--rw-r--r--   0        0        0     2397 2023-08-01 20:45:04.714000 fhirstarter-0.13.9/pyproject.toml
--rw-r--r--   0        0        0     7812 1970-01-01 00:00:00.000000 fhirstarter-0.13.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-25 15:18:03.969523 fhirstarter-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0     6930 2023-08-08 20:21:09.464735 fhirstarter-1.0.0/README.md
+-rw-r--r--   0        0        0      577 2023-08-08 20:21:09.465019 fhirstarter-1.0.0/fhirstarter/__init__.py
+-rw-r--r--   0        0        0     3907 2023-08-08 20:21:09.465897 fhirstarter-1.0.0/fhirstarter/exceptions.py
+-rw-r--r--   0        0        0       92 2023-08-08 20:21:09.466158 fhirstarter-1.0.0/fhirstarter/fhir_specification/__init__.py
+-rw-r--r--   0        0        0     8453 2023-08-08 20:21:09.466416 fhirstarter-1.0.0/fhirstarter/fhir_specification/scripts/download_specification_files.py
+-rw-r--r--   0        0        0        0 2023-08-08 20:21:09.466502 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/R4/__init__.py
+-rw-r--r--   0        0        0   336556 2023-08-08 20:21:09.469140 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/R4/examples.zip
+-rw-r--r--   0        0        0     2814 2023-08-08 20:21:09.469384 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/R4/extra-search-parameters.json
+-rw-r--r--   0        0        0     3334 2023-08-08 20:21:09.469566 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/R4/resources.json
+-rw-r--r--   0        0        0   113904 2023-08-08 20:21:09.470219 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/R4/search-parameters.zip
+-rw-r--r--   0        0        0        0 2023-08-08 20:21:09.470331 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/R4B/__init__.py
+-rw-r--r--   0        0        0   346812 2023-08-08 20:21:09.471036 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/R4B/examples.zip
+-rw-r--r--   0        0        0     1800 2023-08-08 20:21:09.471231 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/R4B/extra-search-parameters.json
+-rw-r--r--   0        0        0     3081 2023-08-08 20:21:09.471380 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/R4B/resources.json
+-rw-r--r--   0        0        0   117431 2023-08-08 20:21:09.472093 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/R4B/search-parameters.zip
+-rw-r--r--   0        0        0        0 2023-08-08 20:21:09.472194 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/R5/__init__.py
+-rw-r--r--   0        0        0   378297 2023-08-08 20:21:09.473817 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/R5/examples.zip
+-rw-r--r--   0        0        0     2356 2023-08-08 20:21:09.474000 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/R5/extra-search-parameters.json
+-rw-r--r--   0        0        0     3526 2023-08-08 20:21:09.474141 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/R5/resources.json
+-rw-r--r--   0        0        0   112399 2023-08-08 20:21:09.474837 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/R5/search-parameters.zip
+-rw-r--r--   0        0        0        0 2023-08-08 20:21:09.474938 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/STU3/__init__.py
+-rw-r--r--   0        0        0   317595 2023-08-08 20:21:09.476420 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/STU3/examples.zip
+-rw-r--r--   0        0        0     2624 2023-08-08 20:21:09.476624 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/STU3/extra-search-parameters.json
+-rw-r--r--   0        0        0     2416 2023-08-08 20:21:09.476767 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/STU3/resources.json
+-rw-r--r--   0        0        0    91155 2023-08-08 20:21:09.477357 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/STU3/search-parameters.zip
+-rw-r--r--   0        0        0       32 2023-08-08 20:21:09.477518 fhirstarter-1.0.0/fhirstarter/fhir_specification/sequences/__init__.py
+-rw-r--r--   0        0        0     4526 2023-08-08 20:21:09.477773 fhirstarter-1.0.0/fhirstarter/fhir_specification/utils.py
+-rw-r--r--   0        0        0    26008 2023-08-08 20:21:09.478140 fhirstarter-1.0.0/fhirstarter/fhirstarter.py
+-rw-r--r--   0        0        0    16957 2023-08-08 20:21:09.479430 fhirstarter-1.0.0/fhirstarter/functions.py
+-rw-r--r--   0        0        0     4769 2023-08-08 20:21:09.480487 fhirstarter-1.0.0/fhirstarter/interactions.py
+-rw-r--r--   0        0        0     6246 2023-08-08 20:21:09.481609 fhirstarter-1.0.0/fhirstarter/providers.py
+-rw-r--r--   0        0        0     1691 2023-08-08 20:21:09.481876 fhirstarter-1.0.0/fhirstarter/resources.py
+-rw-r--r--   0        0        0      151 2023-04-17 15:15:02.746821 fhirstarter-1.0.0/fhirstarter/scripts/config.toml
+-rw-r--r--   0        0        0     4894 2023-08-08 20:21:09.483011 fhirstarter-1.0.0/fhirstarter/scripts/example.py
+-rw-r--r--   0        0        0     6083 2023-08-08 20:21:09.484017 fhirstarter-1.0.0/fhirstarter/search_parameters.py
+-rw-r--r--   0        0        0       68 2022-06-21 20:10:12.695171 fhirstarter-1.0.0/fhirstarter/testclient.py
+-rw-r--r--   0        0        0        0 2022-08-30 15:52:44.718623 fhirstarter-1.0.0/fhirstarter/tests/__init__.py
+-rw-r--r--   0        0        0     4609 2023-08-08 20:21:09.484870 fhirstarter-1.0.0/fhirstarter/tests/config.py
+-rw-r--r--   0        0        0     1244 2023-08-08 20:21:09.485749 fhirstarter-1.0.0/fhirstarter/tests/conftest.py
+-rw-r--r--   0        0        0      814 2023-08-08 20:21:09.486418 fhirstarter-1.0.0/fhirstarter/tests/resources.py
+-rw-r--r--   0        0        0     6622 2023-08-08 20:21:09.487235 fhirstarter-1.0.0/fhirstarter/tests/test_capability_statement.py
+-rw-r--r--   0        0        0     2969 2023-08-08 20:21:09.488185 fhirstarter-1.0.0/fhirstarter/tests/test_dependencies.py
+-rw-r--r--   0        0        0     6605 2023-08-08 20:21:09.489055 fhirstarter-1.0.0/fhirstarter/tests/test_errors.py
+-rw-r--r--   0        0        0    11518 2023-08-08 20:21:09.489875 fhirstarter-1.0.0/fhirstarter/tests/test_interactions.py
+-rw-r--r--   0        0        0     5315 2023-08-06 03:13:57.177101 fhirstarter-1.0.0/fhirstarter/tests/test_utils.py
+-rw-r--r--   0        0        0     2350 2023-08-08 20:21:09.490678 fhirstarter-1.0.0/fhirstarter/tests/utils.py
+-rw-r--r--   0        0        0    17071 2023-08-08 20:29:02.108087 fhirstarter-1.0.0/fhirstarter/utils.py
+-rw-r--r--   0        0        0     2397 2023-08-08 20:31:27.091145 fhirstarter-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8658 1970-01-01 00:00:00.000000 fhirstarter-1.0.0/PKG-INFO
```

### Comparing `fhirstarter-0.13.9/LICENSE.md` & `fhirstarter-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.9/README.md` & `fhirstarter-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -37,344 +37,398 @@
 00000240: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
 00000250: 622e 636f 6d2f 7073 662f 626c 6163 6b22  b.com/psf/black"
 00000260: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
 00000270: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
 00000280: 6c64 732e 696f 2f62 6164 6765 2f63 6f64  lds.io/badge/cod
 00000290: 6525 3230 7374 796c 652d 626c 6163 6b2d  e%20style-black-
 000002a0: 3030 3030 3030 223e 0a20 203c 2f61 3e0a  000000">.  </a>.
-000002b0: 3c2f 703e 0a0a 416e 2041 5347 4920 4648  </p>..An ASGI FH
-000002c0: 4952 2041 5049 2066 7261 6d65 776f 726b  IR API framework
-000002d0: 2062 7569 6c74 206f 6e20 746f 7020 6f66   built on top of
-000002e0: 205b 4661 7374 4150 495d 2868 7474 7073   [FastAPI](https
-000002f0: 3a2f 2f66 6173 7461 7069 2e74 6961 6e67  ://fastapi.tiang
-00000300: 6f6c 6f2e 636f 6d29 2061 6e64 0a5b 4648  olo.com) and.[FH
-00000310: 4952 2052 6573 6f75 7263 6573 5d28 6874  IR Resources](ht
-00000320: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000330: 726f 6a65 6374 2f66 6869 722e 7265 736f  roject/fhir.reso
-00000340: 7572 6365 732f 292e 0a0a 5468 6520 6f6e  urces/)...The on
-00000350: 6c79 2076 6572 7369 6f6e 206f 6620 4648  ly version of FH
-00000360: 4952 2074 6861 7420 6973 2063 7572 7265  IR that is curre
-00000370: 6e74 6c79 2073 7570 706f 7274 6564 2069  ntly supported i
-00000380: 7320 342e 302e 312e 0a0a 2323 2049 6e73  s 4.0.1...## Ins
-00000390: 7461 6c6c 6174 696f 6e0a 0a60 6060 6261  tallation..```ba
-000003a0: 7368 0a70 6970 2069 6e73 7461 6c6c 2066  sh.pip install f
-000003b0: 6869 7273 7461 7274 6572 0a60 6060 0a0a  hirstarter.```..
-000003c0: 2323 2046 6561 7475 7265 730a 0a2a 2041  ## Features..* A
-000003d0: 7574 6f6d 6174 6963 2c20 7374 616e 6461  utomatic, standa
-000003e0: 7264 697a 6564 2041 5049 2072 6f75 7465  rdized API route
-000003f0: 2063 7265 6174 696f 6e0a 2a20 4175 746f   creation.* Auto
-00000400: 6d61 7469 6320 7661 6c69 6461 7469 6f6e  matic validation
-00000410: 206f 6620 696e 7075 7473 2061 6e64 206f   of inputs and o
-00000420: 7574 7075 7473 2074 6872 6f75 6768 2074  utputs through t
-00000430: 6865 2075 7365 206f 6620 4648 4952 2052  he use of FHIR R
-00000440: 6573 6f75 7263 6573 2050 7964 616e 7469  esources Pydanti
-00000450: 6320 6d6f 6465 6c73 0a2a 2041 7574 6f6d  c models.* Autom
-00000460: 6174 6963 616c 6c79 2d67 656e 6572 6174  atically-generat
-00000470: 6564 2063 6170 6162 696c 6974 7920 7374  ed capability st
-00000480: 6174 656d 656e 7420 7468 6174 2063 616e  atement that can
-00000490: 2062 6520 6375 7374 6f6d 697a 6564 2c20   be customized, 
-000004a0: 616e 6420 6120 6361 7061 6269 6c69 7479  and a capability
-000004b0: 2073 7461 7465 6d65 6e74 0a20 2041 5049   statement.  API
-000004c0: 2072 6f75 7465 0a2a 2041 6e20 6578 6365   route.* An exce
-000004d0: 7074 696f 6e2d 6861 6e64 6c69 6e67 2066  ption-handling f
-000004e0: 7261 6d65 776f 726b 2074 6861 7420 7072  ramework that pr
-000004f0: 6f64 7563 6573 2046 4849 522d 6672 6965  oduces FHIR-frie
-00000500: 6e64 6c79 2072 6573 706f 6e73 6573 2028  ndly responses (
-00000510: 692e 652e 204f 7065 7261 7469 6f6e 4f75  i.e. OperationOu
-00000520: 7463 6f6d 6573 290a 2a20 4175 746f 6d61  tcomes).* Automa
-00000530: 7469 6361 6c6c 792d 6765 6e65 7261 7465  tically-generate
-00000540: 642c 2069 6e74 6567 7261 7465 6420 646f  d, integrated do
-00000550: 6375 6d65 6e74 6174 696f 6e20 6765 6e65  cumentation gene
-00000560: 7261 7465 6420 6672 6f6d 2074 6865 2046  rated from the F
-00000570: 4849 5220 7370 6563 6966 6963 6174 696f  HIR specificatio
-00000580: 6e0a 2a20 4375 7374 6f6d 2073 6561 7263  n.* Custom searc
-00000590: 6820 7061 7261 6d65 7465 7273 2066 6f72  h parameters for
-000005a0: 2073 6561 7263 6820 656e 6470 6f69 6e74   search endpoint
-000005b0: 730a 0a23 2323 2044 6973 636c 6169 6d65  s..### Disclaime
-000005c0: 720a 0a46 4849 5253 7461 7274 6572 2077  r..FHIRStarter w
-000005d0: 6173 2062 7569 6c74 2062 6173 6564 206f  as built based o
-000005e0: 6e20 7468 6520 6275 7369 6e65 7373 206e  n the business n
-000005f0: 6565 6473 206f 6620 4361 6e76 6173 204d  eeds of Canvas M
-00000600: 6564 6963 616c 2e20 4174 2061 6e79 2070  edical. At any p
-00000610: 6f69 6e74 2069 6e20 7469 6d65 2c20 6974  oint in time, it
-00000620: 206d 6179 0a6e 6f74 2062 6520 6272 6f61   may.not be broa
-00000630: 646c 7920 6170 706c 6963 6162 6c65 2074  dly applicable t
-00000640: 6f20 7468 6520 696e 6475 7374 7279 2061  o the industry a
-00000650: 7420 6c61 7267 652e 2043 616e 7661 7320  t large. Canvas 
-00000660: 4d65 6469 6361 6c20 6f70 656e 2d73 6f75  Medical open-sou
-00000670: 7263 6564 2074 6865 2070 726f 6a65 6374  rced the project
-00000680: 2073 6f20 7468 6174 0a69 7420 6361 6e20   so that.it can 
-00000690: 6265 2075 7365 6420 6279 2068 6561 6c74  be used by healt
-000006a0: 6863 6172 6520 736f 6674 7761 7265 2064  hcare software d
-000006b0: 6576 656c 6f70 6572 7320 7768 6f73 6520  evelopers whose 
-000006c0: 6e65 6564 7320 6974 206d 6967 6874 2061  needs it might a
-000006d0: 6c73 6f20 6d65 6574 2e20 4f6e 676f 696e  lso meet. Ongoin
-000006e0: 6720 7375 7070 6f72 7420 616e 640a 6465  g support and.de
-000006f0: 7665 6c6f 706d 656e 7420 7769 6c6c 2062  velopment will b
-00000700: 6520 6261 7365 6420 6f6e 2074 6865 2062  e based on the b
-00000710: 7573 696e 6573 7320 6e65 6564 7320 6f66  usiness needs of
-00000720: 2043 616e 7661 7320 4d65 6469 6361 6c2e   Canvas Medical.
-00000730: 0a0a 2323 2042 6163 6b67 726f 756e 640a  ..## Background.
-00000740: 0a46 4849 5253 7461 7274 6572 2075 7365  .FHIRStarter use
-00000750: 7320 6120 7072 6f76 6964 6572 2d64 6563  s a provider-dec
-00000760: 6f72 6174 6f72 2070 6174 7465 726e 2e20  orator pattern. 
-00000770: 4465 7665 6c6f 7065 7273 2063 616e 2077  Developers can w
-00000780: 7269 7465 2066 756e 6374 696f 6e73 2074  rite functions t
-00000790: 6861 7420 696d 706c 656d 656e 7420 4648  hat implement FH
-000007a0: 4952 0a69 6e74 6572 6163 7469 6f6e 7320  IR.interactions 
-000007b0: 2d2d 2073 7563 6820 6173 2063 7265 6174  -- such as creat
-000007c0: 652c 2072 6561 642c 2073 6561 7263 682d  e, read, search-
-000007d0: 7479 7065 2c20 616e 6420 7570 6461 7465  type, and update
-000007e0: 202d 2d20 616e 6420 706c 7567 2074 6865   -- and plug the
-000007f0: 6d20 696e 746f 2074 6865 2066 7261 6d65  m into the frame
-00000800: 776f 726b 2e0a 4648 4952 5374 6172 7465  work..FHIRStarte
-00000810: 7220 7468 656e 2061 7574 6f6d 6174 6963  r then automatic
-00000820: 616c 6c79 2063 7265 6174 6573 2046 4849  ally creates FHI
-00000830: 522d 636f 6d70 6174 6962 6c65 2041 5049  R-compatible API
-00000840: 2072 6f75 7465 7320 6672 6f6d 2074 6865   routes from the
-00000850: 7365 2064 6576 656c 6f70 6572 2d70 726f  se developer-pro
-00000860: 7669 6465 640a 6675 6e63 7469 6f6e 732e  vided.functions.
-00000870: 2046 4849 5220 696e 7465 7261 6374 696f   FHIR interactio
-00000880: 6e73 2074 6861 7420 6172 6520 7375 7070  ns that are supp
-00000890: 6c69 6564 206d 7573 7420 7573 6520 7468  lied must use th
-000008a0: 6520 7265 736f 7572 6365 2063 6c61 7373  e resource class
-000008b0: 6573 2064 6566 696e 6564 2062 7920 7468  es defined by th
-000008c0: 650a 5b46 4849 5220 5265 736f 7572 6365  e.[FHIR Resource
-000008d0: 735d 2868 7474 7073 3a2f 2f70 7970 692e  s](https://pypi.
-000008e0: 6f72 672f 7072 6f6a 6563 742f 6668 6972  org/project/fhir
-000008f0: 2e72 6573 6f75 7263 6573 2f29 2050 7974  .resources/) Pyt
-00000900: 686f 6e20 7061 636b 6167 652c 2077 6869  hon package, whi
-00000910: 6368 2069 7320 6120 636f 6c6c 6563 7469  ch is a collecti
-00000920: 6f6e 206f 660a 5079 6461 6e74 6963 206d  on of.Pydantic m
-00000930: 6f64 656c 7320 666f 7220 4648 4952 2072  odels for FHIR r
-00000940: 6573 6f75 7263 6573 2e0a 0a49 6e20 6f72  esources...In or
-00000950: 6465 7220 746f 2073 7461 6e64 2075 7020  der to stand up 
-00000960: 6120 4648 4952 2073 6572 7665 722c 2061  a FHIR server, a
-00000970: 6c6c 2074 6861 7420 6973 2072 6571 7569  ll that is requi
-00000980: 7265 6420 6973 2074 6f20 6372 6561 7465  red is to create
-00000990: 2061 2046 4849 5253 7461 7274 6572 2061   a FHIRStarter a
-000009a0: 6e64 2061 0a46 4849 5250 726f 7669 6465  nd a.FHIRProvide
-000009b0: 7220 696e 7374 616e 6365 2c20 7265 6769  r instance, regi
-000009c0: 7374 6572 2061 2046 4849 5220 696e 7465  ster a FHIR inte
-000009d0: 7261 6374 696f 6e20 7769 7468 2074 6865  raction with the
-000009e0: 2070 726f 7669 6465 722c 2061 6464 2074   provider, add t
-000009f0: 6865 2070 726f 7669 6465 7220 746f 2074  he provider to t
-00000a00: 6865 0a46 4849 5253 7461 7274 6572 2069  he.FHIRStarter i
-00000a10: 6e73 7461 6e63 652c 2061 6e64 2070 6173  nstance, and pas
-00000a20: 7320 7468 6520 4648 4952 5374 6172 7465  s the FHIRStarte
-00000a30: 7220 696e 7374 616e 6365 2074 6f20 616e  r instance to an
-00000a40: 2041 5347 4920 7365 7276 6572 2e0a 0a23   ASGI server...#
-00000a50: 2320 5573 6167 650a 0a23 2323 2043 7572  # Usage..### Cur
-00000a60: 7265 6e74 6c79 2d73 7570 706f 7274 6564  rently-supported
-00000a70: 2066 756e 6374 696f 6e61 6c69 7479 0a0a   functionality..
-00000a80: 4648 4952 5374 6172 7465 7220 7375 7070  FHIRStarter supp
-00000a90: 6f72 7473 2063 7265 6174 652c 2072 6561  orts create, rea
-00000aa0: 642c 2073 6561 7263 682d 7479 7065 2c20  d, search-type, 
-00000ab0: 616e 6420 7570 6461 7465 2065 6e64 706f  and update endpo
-00000ac0: 696e 7473 2061 6372 6f73 7320 616c 6c20  ints across all 
-00000ad0: 4648 4952 2052 3420 7265 736f 7572 6365  FHIR R4 resource
-00000ae0: 0a74 7970 6573 2c20 616e 6420 7769 6c6c  .types, and will
-00000af0: 2061 7574 6f6d 6174 6963 616c 6c79 2067   automatically g
-00000b00: 656e 6572 6174 6520 7468 6520 602f 6d65  enerate the `/me
-00000b10: 7461 6461 7461 6020 6361 7061 6269 6c69  tadata` capabili
-00000b20: 7469 6573 2073 7461 7465 6d65 6e74 2065  ties statement e
-00000b30: 6e64 706f 696e 742e 0a0a 2323 2320 4578  ndpoint...### Ex
-00000b40: 616d 706c 650a 0a41 2064 6574 6169 6c65  ample..A detaile
-00000b50: 6420 6578 616d 706c 6520 6973 2061 7661  d example is ava
-00000b60: 696c 6162 6c65 2068 6572 653a 205b 6578  ilable here: [ex
-00000b70: 616d 706c 652e 7079 5d28 6874 7470 733a  ample.py](https:
-00000b80: 2f2f 6769 7468 7562 2e63 6f6d 2f63 616e  //github.com/can
-00000b90: 7661 732d 6d65 6469 6361 6c2f 6668 6972  vas-medical/fhir
-00000ba0: 7374 6172 7465 722f 626c 6f62 2f6d 6169  starter/blob/mai
-00000bb0: 6e2f 6668 6972 7374 6172 7465 722f 7363  n/fhirstarter/sc
-00000bc0: 7269 7074 732f 6578 616d 706c 652e 7079  ripts/example.py
-00000bd0: 292e 0a0a 6060 6070 7974 686f 6e0a 696d  )...```python.im
-00000be0: 706f 7274 2075 7669 636f 726e 0a66 726f  port uvicorn.fro
-00000bf0: 6d20 6668 6972 2e72 6573 6f75 7263 6573  m fhir.resources
-00000c00: 2e66 6869 7274 7970 6573 2069 6d70 6f72  .fhirtypes impor
-00000c10: 7420 4964 0a66 726f 6d20 6668 6972 2e72  t Id.from fhir.r
-00000c20: 6573 6f75 7263 6573 2e70 6174 6965 6e74  esources.patient
-00000c30: 2069 6d70 6f72 7420 5061 7469 656e 740a   import Patient.
-00000c40: 0a66 726f 6d20 6668 6972 7374 6172 7465  .from fhirstarte
-00000c50: 7220 696d 706f 7274 2046 4849 5250 726f  r import FHIRPro
-00000c60: 7669 6465 722c 2046 4849 5253 7461 7274  vider, FHIRStart
-00000c70: 6572 2c20 496e 7465 7261 6374 696f 6e43  er, InteractionC
-00000c80: 6f6e 7465 7874 0a66 726f 6d20 6668 6972  ontext.from fhir
-00000c90: 7374 6172 7465 722e 6578 6365 7074 696f  starter.exceptio
-00000ca0: 6e73 2069 6d70 6f72 7420 4648 4952 5265  ns import FHIRRe
-00000cb0: 736f 7572 6365 4e6f 7446 6f75 6e64 4572  sourceNotFoundEr
-00000cc0: 726f 720a 0a23 2043 7265 6174 6520 7468  ror..# Create th
-00000cd0: 6520 6170 700a 6170 7020 3d20 4648 4952  e app.app = FHIR
-00000ce0: 5374 6172 7465 7228 290a 0a23 2043 7265  Starter()..# Cre
-00000cf0: 6174 6520 6120 7072 6f76 6964 6572 0a70  ate a provider.p
-00000d00: 726f 7669 6465 7220 3d20 4648 4952 5072  rovider = FHIRPr
-00000d10: 6f76 6964 6572 2829 0a0a 0a23 2052 6567  ovider()...# Reg
-00000d20: 6973 7465 7220 7468 6520 7061 7469 656e  ister the patien
-00000d30: 7420 7265 6164 2046 4849 5220 696e 7465  t read FHIR inte
-00000d40: 7261 6374 696f 6e20 7769 7468 2074 6865  raction with the
-00000d50: 2070 726f 7669 6465 720a 4070 726f 7669   provider.@provi
-00000d60: 6465 722e 7265 6164 2850 6174 6965 6e74  der.read(Patient
-00000d70: 290a 6173 796e 6320 6465 6620 7061 7469  ).async def pati
-00000d80: 656e 745f 7265 6164 2863 6f6e 7465 7874  ent_read(context
-00000d90: 3a20 496e 7465 7261 6374 696f 6e43 6f6e  : InteractionCon
-00000da0: 7465 7874 2c20 6964 5f3a 2049 6429 202d  text, id_: Id) -
-00000db0: 3e20 5061 7469 656e 743a 0a20 2020 2023  > Patient:.    #
-00000dc0: 2047 6574 2074 6865 2070 6174 6965 6e74   Get the patient
-00000dd0: 2066 726f 6d20 7468 6520 6461 7461 6261   from the databa
-00000de0: 7365 0a20 2020 2070 6174 6965 6e74 203d  se.    patient =
-00000df0: 202e 2e2e 0a0a 2020 2020 6966 206e 6f74   .....    if not
-00000e00: 2070 6174 6965 6e74 3a0a 2020 2020 2020   patient:.      
-00000e10: 2020 7261 6973 6520 4648 4952 5265 736f    raise FHIRReso
-00000e20: 7572 6365 4e6f 7446 6f75 6e64 4572 726f  urceNotFoundErro
-00000e30: 720a 0a20 2020 2072 6574 7572 6e20 5061  r..    return Pa
-00000e40: 7469 656e 7428 0a20 2020 2020 2020 202a  tient(.        *
-00000e50: 2a7b 0a20 2020 2020 2020 2020 2020 2023  *{.            #
-00000e60: 204d 6170 2070 6174 6965 6e74 2066 726f   Map patient fro
-00000e70: 6d20 6461 7461 6261 7365 2074 6f20 4648  m database to FH
-00000e80: 4952 2050 6174 6965 6e74 2073 7472 7563  IR Patient struc
-00000e90: 7475 7265 0a20 2020 2020 2020 207d 0a20  ture.        }. 
-00000ea0: 2020 2029 0a0a 0a23 2041 6464 2074 6865     )...# Add the
-00000eb0: 2070 726f 7669 6465 7220 746f 2074 6865   provider to the
-00000ec0: 2061 7070 0a61 7070 2e61 6464 5f70 726f   app.app.add_pro
-00000ed0: 7669 6465 7273 2870 726f 7669 6465 7229  viders(provider)
-00000ee0: 0a0a 0a69 6620 5f5f 6e61 6d65 5f5f 203d  ...if __name__ =
-00000ef0: 3d20 225f 5f6d 6169 6e5f 5f22 3a0a 2020  = "__main__":.  
-00000f00: 2020 2320 5374 6172 7420 7468 6520 7365    # Start the se
-00000f10: 7276 6572 0a20 2020 2075 7669 636f 726e  rver.    uvicorn
-00000f20: 2e72 756e 2861 7070 290a 6060 600a 0a23  .run(app).```..#
-00000f30: 2323 2043 7573 746f 6d20 7365 6172 6368  ## Custom search
-00000f40: 2070 6172 616d 6574 6572 730a 0a43 7573   parameters..Cus
-00000f50: 746f 6d20 7365 6172 6368 2070 6172 616d  tom search param
-00000f60: 6574 6572 7320 6361 6e20 6265 2064 6566  eters can be def
-00000f70: 696e 6564 2069 6e20 6120 636f 6e66 6967  ined in a config
-00000f80: 7572 6174 696f 6e20 6669 6c65 2074 6861  uration file tha
-00000f90: 7420 6361 6e20 6265 2070 6173 7365 6420  t can be passed 
-00000fa0: 746f 2074 6865 2061 7070 206f 6e0a 6372  to the app on.cr
-00000fb0: 6561 7469 6f6e 2e0a 0a60 6060 746f 6d6c  eation...```toml
-00000fc0: 0a5b 7365 6172 6368 2d70 6172 616d 6574  .[search-paramet
-00000fd0: 6572 732e 5061 7469 656e 742e 6e69 636b  ers.Patient.nick
-00000fe0: 6e61 6d65 5d0a 7479 7065 203d 2022 7374  name].type = "st
-00000ff0: 7269 6e67 220a 6465 7363 7269 7074 696f  ring".descriptio
-00001000: 6e20 3d20 224e 6963 6b6e 616d 6522 0a75  n = "Nickname".u
-00001010: 7269 203d 2022 6874 7470 733a 2f2f 686f  ri = "https://ho
-00001020: 7374 6e61 6d65 2f6e 6963 6b6e 616d 6522  stname/nickname"
-00001030: 0a69 6e63 6c75 6465 2d69 6e2d 6361 7061  .include-in-capa
-00001040: 6269 6c69 7479 2d73 7461 7465 6d65 6e74  bility-statement
-00001050: 203d 2074 7275 650a 6060 600a 0a41 6464   = true.```..Add
-00001060: 696e 6720 6120 6375 7374 6f6d 2073 6561  ing a custom sea
-00001070: 7263 6820 7061 7261 6d65 7465 7220 7669  rch parameter vi
-00001080: 6120 636f 6e66 6967 7572 6174 696f 6e20  a configuration 
-00001090: 616c 6c6f 7773 2074 6869 7320 6e61 6d65  allows this name
-000010a0: 2074 6f20 6265 2075 7365 6420 6173 2061   to be used as a
-000010b0: 6e20 6172 6775 6d65 6e74 2077 6865 6e0a  n argument when.
-000010c0: 6465 6669 6e69 6e67 2061 2073 6561 7263  defining a searc
-000010d0: 682d 7479 7065 2069 6e74 6572 6163 7469  h-type interacti
-000010e0: 6f6e 2068 616e 646c 6572 2061 6e64 2061  on handler and a
-000010f0: 6c73 6f20 6164 6473 2074 6869 7320 7365  lso adds this se
-00001100: 6172 6368 2070 6172 616d 6574 6572 2074  arch parameter t
-00001110: 6f20 7468 6520 4150 490a 646f 6375 6d65  o the API.docume
-00001120: 6e74 6174 696f 6e20 666f 7220 7468 6520  ntation for the 
-00001130: 7365 6172 6368 2065 6e64 706f 696e 742e  search endpoint.
-00001140: 0a0a 2323 2320 4361 7061 6269 6c69 7479  ..### Capability
-00001150: 2073 7461 7465 6d65 6e74 0a0a 4974 2069   statement..It i
-00001160: 7320 706f 7373 6962 6c65 2074 6f20 6375  s possible to cu
-00001170: 7374 6f6d 697a 6520 7468 6520 6361 7061  stomize the capa
-00001180: 6269 6c69 7479 2073 7461 7465 6d65 6e74  bility statement
-00001190: 2062 7920 7365 7474 696e 6720 6120 6361   by setting a ca
-000011a0: 7061 6269 6c69 7479 2073 7461 7465 6d65  pability stateme
-000011b0: 6e74 206d 6f64 6966 6965 723a 0a0a 6060  nt modifier:..``
-000011c0: 6070 7974 686f 6e0a 6465 6620 616d 656e  `python.def amen
-000011d0: 645f 6361 7061 6269 6c69 7479 5f73 7461  d_capability_sta
-000011e0: 7465 6d65 6e74 280a 2020 2020 6361 7061  tement(.    capa
-000011f0: 6269 6c69 7479 5f73 7461 7465 6d65 6e74  bility_statement
-00001200: 3a20 4d75 7461 626c 654d 6170 7069 6e67  : MutableMapping
-00001210: 5b73 7472 2c20 416e 795d 2c20 7265 7175  [str, Any], requ
-00001220: 6573 743a 2052 6571 7565 7374 2c20 7265  est: Request, re
-00001230: 7370 6f6e 7365 3a20 5265 7370 6f6e 7365  sponse: Response
-00001240: 0a29 202d 3e20 4d75 7461 626c 654d 6170  .) -> MutableMap
-00001250: 7069 6e67 5b73 7472 2c20 416e 795d 3a0a  ping[str, Any]:.
-00001260: 2020 2020 6361 7061 6269 6c69 7479 5f73      capability_s
-00001270: 7461 7465 6d65 6e74 5b22 7075 626c 6973  tatement["publis
-00001280: 6865 7222 5d20 3d20 2243 616e 7661 7320  her"] = "Canvas 
-00001290: 4d65 6469 6361 6c22 0a20 2020 2072 6574  Medical".    ret
-000012a0: 7572 6e20 6361 7061 6269 6c69 7479 5f73  urn capability_s
-000012b0: 7461 7465 6d65 6e74 0a0a 6170 702e 7365  tatement..app.se
-000012c0: 745f 6361 7061 6269 6c69 7479 5f73 7461  t_capability_sta
-000012d0: 7465 6d65 6e74 5f6d 6f64 6966 6965 7228  tement_modifier(
-000012e0: 616d 656e 645f 6361 7061 6269 6c69 7479  amend_capability
-000012f0: 5f73 7461 7465 6d65 6e74 290a 6060 600a  _statement).```.
-00001300: 0a23 2323 2046 6173 7441 5049 2064 6570  .### FastAPI dep
-00001310: 656e 6465 6e63 7920 696e 6a65 6374 696f  endency injectio
-00001320: 6e0a 0a46 6173 7441 5049 2773 2064 6570  n..FastAPI's dep
-00001330: 656e 6465 6e63 7920 696e 6a65 6374 696f  endency injectio
-00001340: 6e20 6973 2065 7870 6f73 6564 2061 7420  n is exposed at 
-00001350: 7661 7269 6f75 7320 6c65 7665 6c73 3a0a  various levels:.
-00001360: 0a2a 202a 2a61 7070 6c69 6361 7469 6f6e  .* **application
-00001370: 2a2a 3a20 7468 6520 605f 5f69 6e69 745f  **: the `__init_
-00001380: 5f60 206d 6574 686f 6420 6f6e 2074 6865  _` method on the
-00001390: 2046 4849 5253 7461 7274 6572 2063 6c61   FHIRStarter cla
-000013a0: 7373 0a2a 202a 2a70 726f 7669 6465 722a  ss.* **provider*
-000013b0: 2a3a 2074 6865 2060 5f5f 696e 6974 5f5f  *: the `__init__
-000013c0: 6020 6d65 7468 6f64 206f 6e20 7468 6520  ` method on the 
-000013d0: 4648 4952 5072 6f76 6964 6572 2063 6c61  FHIRProvider cla
-000013e0: 7373 0a2a 202a 2a68 616e 646c 6572 2a2a  ss.* **handler**
-000013f0: 3a20 7468 6520 6063 7265 6174 6560 2c20  : the `create`, 
-00001400: 6072 6561 6460 2c20 6073 6561 7263 685f  `read`, `search_
-00001410: 7479 7065 602c 206f 7220 6075 7064 6174  type`, or `updat
-00001420: 6560 2064 6563 6f72 6174 6f72 2075 7365  e` decorator use
-00001430: 6420 746f 2061 6464 2061 2068 616e 646c  d to add a handl
-00001440: 6572 2074 6f20 6120 7072 6f76 6964 6572  er to a provider
-00001450: 0a0a 4465 7065 6e64 656e 6369 6573 2073  ..Dependencies s
-00001460: 7065 6369 6669 6564 2061 7420 7468 6520  pecified at the 
-00001470: 6170 706c 6963 6174 696f 6e20 6c65 7665  application leve
-00001480: 6c20 7769 6c6c 2062 6520 696e 6a65 6374  l will be inject
-00001490: 6564 2069 6e74 6f20 616c 6c20 726f 7574  ed into all rout
-000014a0: 6573 2069 6e20 7468 6520 6170 706c 6963  es in the applic
-000014b0: 6174 696f 6e2e 0a0a 4465 7065 6e64 656e  ation...Dependen
-000014c0: 6369 6573 2073 7065 6369 6669 6564 2061  cies specified a
-000014d0: 7420 7468 6520 7072 6f76 6964 6572 206c  t the provider l
-000014e0: 6576 656c 2077 696c 6c20 6265 2069 6e6a  evel will be inj
-000014f0: 6563 7465 6420 696e 746f 2061 6c6c 2072  ected into all r
-00001500: 6f75 7465 7320 7468 6174 2061 7265 2061  outes that are a
-00001510: 6464 6564 2074 6f0a 7468 6520 6170 706c  dded to.the appl
-00001520: 6963 6174 696f 6e20 6672 6f6d 2074 6861  ication from tha
-00001530: 7420 7370 6563 6966 6963 2070 726f 7669  t specific provi
-00001540: 6465 722e 0a0a 4465 7065 6e64 656e 6369  der...Dependenci
-00001550: 6573 2073 7065 6369 6669 6564 2061 7420  es specified at 
-00001560: 7468 6520 6861 6e64 6c65 7220 6c65 7665  the handler leve
-00001570: 6c20 6f6e 6c79 2061 7070 6c79 2074 6f20  l only apply to 
-00001580: 7468 6174 2073 7065 6369 6669 6320 4648  that specific FH
-00001590: 4952 2069 6e74 6572 6163 7469 6f6e 2e0a  IR interaction..
-000015a0: 0a23 2320 466f 7277 6172 6420 636f 6d70  .## Forward comp
-000015b0: 6174 6962 696c 6974 790a 0a41 7420 736f  atibility..At so
-000015c0: 6d65 2070 6f69 6e74 2069 6e20 7468 6520  me point in the 
-000015d0: 6675 7475 7265 2c20 6974 2077 696c 6c20  future, it will 
-000015e0: 6265 206e 6563 6573 7361 7279 2074 6f20  be necessary to 
-000015f0: 7375 7070 6f72 7420 4648 4952 2052 352e  support FHIR R5.
-00001600: 2048 6f77 2074 6869 7320 6d69 6768 7420   How this might 
-00001610: 6265 2073 7570 706f 7274 6564 206f 6e0a  be supported on.
-00001620: 6120 7365 7276 6572 2074 6861 7420 636f  a server that co
-00001630: 6e74 696e 7565 7320 746f 2073 7570 706f  ntinues to suppo
-00001640: 7274 2052 3420 6861 7320 6e6f 7420 7965  rt R4 has not ye
-00001650: 7420 6265 656e 2064 6574 6572 6d69 6e65  t been determine
-00001660: 6420 2865 2e67 2e20 6120 6865 6164 6572  d (e.g. a header
-00001670: 2074 6861 7420 7370 6563 6966 6965 7320   that specifies 
-00001680: 7468 650a 7665 7273 696f 6e2c 2061 6464  the.version, add
-00001690: 696e 6720 7468 6520 4648 4952 2076 6572  ing the FHIR ver
-000016a0: 7369 6f6e 2074 6f20 7468 6520 5552 4c20  sion to the URL 
-000016b0: 7061 7468 2c20 6574 632e 292e 2049 7420  path, etc.). It 
-000016c0: 6d61 7920 6265 206e 6563 6573 7361 7279  may be necessary
-000016d0: 2074 6f20 7375 7070 6f72 7420 616c 7465   to support alte
-000016e0: 7261 7469 6f6e 0a6f 6620 686f 7720 7468  ration.of how th
-000016f0: 6520 5552 4c20 7061 7468 2069 7320 7370  e URL path is sp
-00001700: 6563 6966 6965 6420 7468 726f 7567 6820  ecified through 
-00001710: 7468 6520 7072 6f76 6964 6572 2063 6f6e  the provider con
-00001720: 7374 7275 6374 2e20 4375 7272 656e 746c  struct. Currentl
-00001730: 792c 2074 6865 2046 4849 5220 7665 7273  y, the FHIR vers
-00001740: 696f 6e20 6973 206e 6f74 0a70 6172 7420  ion is not.part 
-00001750: 6f66 2074 6865 2055 524c 2070 6174 682c  of the URL path,
-00001760: 2073 6f20 7468 6520 6465 6661 756c 7420   so the default 
-00001770: 6265 6861 7669 6f72 2069 7320 7468 6174  behavior is that
-00001780: 2061 6e20 4150 4920 726f 7574 6520 6465   an API route de
-00001790: 6669 6e65 6420 6173 2060 2f50 6174 6965  fined as `/Patie
-000017a0: 6e74 6020 7769 6c6c 2062 6520 616e 0a52  nt` will be an.R
-000017b0: 3420 656e 6470 6f69 6e74 2e0a            4 endpoint..
+000002b0: 3c2f 703e 0a0a 416e 2041 5347 4920 5b46  </p>..An ASGI [F
+000002c0: 4849 525d 2868 7474 7073 3a2f 2f68 6c37  HIR](https://hl7
+000002d0: 2e6f 7267 2f66 6869 722f 2920 4150 4920  .org/fhir/) API 
+000002e0: 6672 616d 6577 6f72 6b20 6275 696c 7420  framework built 
+000002f0: 6f6e 2074 6f70 206f 6620 5b46 6173 7441  on top of [FastA
+00000300: 5049 5d28 6874 7470 733a 2f2f 6661 7374  PI](https://fast
+00000310: 6170 692e 7469 616e 676f 6c6f 2e63 6f6d  api.tiangolo.com
+00000320: 2920 616e 640a 5b46 4849 5220 5265 736f  ) and.[FHIR Reso
+00000330: 7572 6365 735d 2868 7474 7073 3a2f 2f70  urces](https://p
+00000340: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00000350: 6668 6972 2e72 6573 6f75 7263 6573 2f29  fhir.resources/)
+00000360: 2e0a 0a53 7570 706f 7274 7320 4648 4952  ...Supports FHIR
+00000370: 2073 6571 7565 6e63 6573 3a0a 2a20 5b53   sequences:.* [S
+00000380: 5455 2028 7633 2e30 2e32 295d 2868 7474  TU (v3.0.2)](htt
+00000390: 7073 3a2f 2f68 6c37 2e6f 7267 2f66 6869  ps://hl7.org/fhi
+000003a0: 722f 5354 5533 2f29 0a2a 205b 5234 2028  r/STU3/).* [R4 (
+000003b0: 7634 2e30 2e31 295d 2868 7474 7073 3a2f  v4.0.1)](https:/
+000003c0: 2f68 6c37 2e6f 7267 2f66 6869 722f 5234  /hl7.org/fhir/R4
+000003d0: 2f29 0a2a 205b 5234 4220 2876 342e 332e  /).* [R4B (v4.3.
+000003e0: 3029 5d28 6874 7470 733a 2f2f 686c 372e  0)](https://hl7.
+000003f0: 6f72 672f 6668 6972 2f52 3442 2f29 0a2a  org/fhir/R4B/).*
+00000400: 205b 5235 2028 7635 2e30 2e30 295d 2868   [R5 (v5.0.0)](h
+00000410: 7474 7073 3a2f 2f68 6c37 2e6f 7267 2f66  ttps://hl7.org/f
+00000420: 6869 722f 5235 2f29 0a0a 2323 2049 6e73  hir/R5/)..## Ins
+00000430: 7461 6c6c 6174 696f 6e0a 0a60 6060 6261  tallation..```ba
+00000440: 7368 0a70 6970 2069 6e73 7461 6c6c 2066  sh.pip install f
+00000450: 6869 7273 7461 7274 6572 0a60 6060 0a0a  hirstarter.```..
+00000460: 2323 2046 6561 7475 7265 730a 0a2a 2041  ## Features..* A
+00000470: 7574 6f6d 6174 6963 2c20 7374 616e 6461  utomatic, standa
+00000480: 7264 697a 6564 2041 5049 2072 6f75 7465  rdized API route
+00000490: 2063 7265 6174 696f 6e0a 2a20 4175 746f   creation.* Auto
+000004a0: 6d61 7469 6320 7661 6c69 6461 7469 6f6e  matic validation
+000004b0: 206f 6620 696e 7075 7473 2061 6e64 206f   of inputs and o
+000004c0: 7574 7075 7473 2074 6872 6f75 6768 2074  utputs through t
+000004d0: 6865 2075 7365 206f 6620 4648 4952 2052  he use of FHIR R
+000004e0: 6573 6f75 7263 6573 2050 7964 616e 7469  esources Pydanti
+000004f0: 6320 6d6f 6465 6c73 0a2a 2041 7574 6f6d  c models.* Autom
+00000500: 6174 6963 616c 6c79 2d67 656e 6572 6174  atically-generat
+00000510: 6564 2063 6170 6162 696c 6974 7920 7374  ed capability st
+00000520: 6174 656d 656e 7420 7468 6174 2063 616e  atement that can
+00000530: 2062 6520 6375 7374 6f6d 697a 6564 2c20   be customized, 
+00000540: 616e 6420 6120 6361 7061 6269 6c69 7479  and a capability
+00000550: 2073 7461 7465 6d65 6e74 0a20 2041 5049   statement.  API
+00000560: 2072 6f75 7465 0a2a 2041 6e20 6578 6365   route.* An exce
+00000570: 7074 696f 6e2d 6861 6e64 6c69 6e67 2066  ption-handling f
+00000580: 7261 6d65 776f 726b 2074 6861 7420 7072  ramework that pr
+00000590: 6f64 7563 6573 2046 4849 522d 6672 6965  oduces FHIR-frie
+000005a0: 6e64 6c79 2072 6573 706f 6e73 6573 2028  ndly responses (
+000005b0: 692e 652e 204f 7065 7261 7469 6f6e 4f75  i.e. OperationOu
+000005c0: 7463 6f6d 6573 290a 2a20 4175 746f 6d61  tcomes).* Automa
+000005d0: 7469 6361 6c6c 792d 6765 6e65 7261 7465  tically-generate
+000005e0: 642c 2069 6e74 6567 7261 7465 6420 646f  d, integrated do
+000005f0: 6375 6d65 6e74 6174 696f 6e20 6765 6e65  cumentation gene
+00000600: 7261 7465 6420 6672 6f6d 2074 6865 2046  rated from the F
+00000610: 4849 5220 7370 6563 6966 6963 6174 696f  HIR specificatio
+00000620: 6e0a 2a20 4375 7374 6f6d 2073 6561 7263  n.* Custom searc
+00000630: 6820 7061 7261 6d65 7465 7273 2066 6f72  h parameters for
+00000640: 2073 6561 7263 6820 656e 6470 6f69 6e74   search endpoint
+00000650: 730a 0a23 2323 2044 6973 636c 6169 6d65  s..### Disclaime
+00000660: 720a 0a46 4849 5253 7461 7274 6572 2077  r..FHIRStarter w
+00000670: 6173 2062 7569 6c74 2062 6173 6564 206f  as built based o
+00000680: 6e20 7468 6520 6275 7369 6e65 7373 206e  n the business n
+00000690: 6565 6473 206f 660a 5b43 616e 7661 7320  eeds of.[Canvas 
+000006a0: 4d65 6469 6361 6c5d 2868 7474 7073 3a2f  Medical](https:/
+000006b0: 2f77 7777 2e63 616e 7661 736d 6564 6963  /www.canvasmedic
+000006c0: 616c 2e63 6f6d 292e 2041 7420 616e 7920  al.com). At any 
+000006d0: 706f 696e 7420 696e 2074 696d 652c 2069  point in time, i
+000006e0: 7420 6d61 7920 6e6f 7420 6265 2062 726f  t may not be bro
+000006f0: 6164 6c79 0a61 7070 6c69 6361 626c 6520  adly.applicable 
+00000700: 746f 2074 6865 2069 6e64 7573 7472 7920  to the industry 
+00000710: 6174 206c 6172 6765 2e20 4361 6e76 6173  at large. Canvas
+00000720: 204d 6564 6963 616c 206f 7065 6e2d 736f   Medical open-so
+00000730: 7572 6365 6420 7468 6520 7072 6f6a 6563  urced the projec
+00000740: 7420 736f 2074 6861 7420 6974 2063 616e  t so that it can
+00000750: 2062 6520 7573 6564 0a62 7920 6865 616c   be used.by heal
+00000760: 7468 6361 7265 2073 6f66 7477 6172 6520  thcare software 
+00000770: 6465 7665 6c6f 7065 7273 2077 686f 7365  developers whose
+00000780: 206e 6565 6473 2069 7420 6d69 6768 7420   needs it might 
+00000790: 616c 736f 206d 6565 742e 204f 6e67 6f69  also meet. Ongoi
+000007a0: 6e67 2073 7570 706f 7274 2061 6e64 2064  ng support and d
+000007b0: 6576 656c 6f70 6d65 6e74 0a77 696c 6c20  evelopment.will 
+000007c0: 6265 2062 6173 6564 206f 6e20 7468 6520  be based on the 
+000007d0: 6275 7369 6e65 7373 206e 6565 6473 206f  business needs o
+000007e0: 6620 4361 6e76 6173 204d 6564 6963 616c  f Canvas Medical
+000007f0: 2e0a 0a23 2320 4261 636b 6772 6f75 6e64  ...## Background
+00000800: 0a0a 4648 4952 5374 6172 7465 7220 7573  ..FHIRStarter us
+00000810: 6573 2061 2070 726f 7669 6465 722d 6465  es a provider-de
+00000820: 636f 7261 746f 7220 7061 7474 6572 6e2e  corator pattern.
+00000830: 2044 6576 656c 6f70 6572 7320 6361 6e20   Developers can 
+00000840: 7772 6974 6520 6675 6e63 7469 6f6e 732c  write functions,
+00000850: 206f 7220 6861 6e64 6c65 7273 2c20 7468   or handlers, th
+00000860: 6174 0a69 6d70 6c65 6d65 6e74 2046 4849  at.implement FHI
+00000870: 5220 696e 7465 7261 6374 696f 6e73 202d  R interactions -
+00000880: 2d20 7375 6368 2061 7320 6372 6561 7465  - such as create
+00000890: 2c20 7265 6164 2c20 7365 6172 6368 2d74  , read, search-t
+000008a0: 7970 652c 2061 6e64 2075 7064 6174 6520  ype, and update 
+000008b0: 2d2d 2061 6e64 2070 6c75 6720 7468 656d  -- and plug them
+000008c0: 2069 6e74 6f0a 7468 6520 6672 616d 6577   into.the framew
+000008d0: 6f72 6b2e 2046 4849 5253 7461 7274 6572  ork. FHIRStarter
+000008e0: 2074 6865 6e20 6175 746f 6d61 7469 6361   then automatica
+000008f0: 6c6c 7920 6372 6561 7465 7320 4648 4952  lly creates FHIR
+00000900: 2d63 6f6d 7061 7469 626c 6520 4150 4920  -compatible API 
+00000910: 726f 7574 6573 2066 726f 6d20 7468 6573  routes from thes
+00000920: 650a 6465 7665 6c6f 7065 722d 7072 6f76  e.developer-prov
+00000930: 6964 6564 2066 756e 6374 696f 6e73 2e20  ided functions. 
+00000940: 4648 4952 2069 6e74 6572 6163 7469 6f6e  FHIR interaction
+00000950: 7320 7468 6174 2061 7265 2073 7570 706c  s that are suppl
+00000960: 6965 6420 6d75 7374 2075 7365 2074 6865  ied must use the
+00000970: 2072 6573 6f75 7263 6520 636c 6173 7365   resource classe
+00000980: 730a 6465 6669 6e65 6420 6279 2074 6865  s.defined by the
+00000990: 205b 4648 4952 2052 6573 6f75 7263 6573   [FHIR Resources
+000009a0: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
+000009b0: 7267 2f70 726f 6a65 6374 2f66 6869 722e  rg/project/fhir.
+000009c0: 7265 736f 7572 6365 732f 2920 5079 7468  resources/) Pyth
+000009d0: 6f6e 2070 6163 6b61 6765 2c20 7768 6963  on package, whic
+000009e0: 6820 6973 2061 0a63 6f6c 6c65 6374 696f  h is a.collectio
+000009f0: 6e20 6f66 2050 7964 616e 7469 6320 6d6f  n of Pydantic mo
+00000a00: 6465 6c73 2066 6f72 2046 4849 5220 7265  dels for FHIR re
+00000a10: 736f 7572 6365 732e 0a0a 496e 206f 7264  sources...In ord
+00000a20: 6572 2074 6f20 7374 616e 6420 7570 2061  er to stand up a
+00000a30: 2046 4849 5220 7365 7276 6572 2c20 616c   FHIR server, al
+00000a40: 6c20 7468 6174 2069 7320 7265 7175 6972  l that is requir
+00000a50: 6564 2069 7320 746f 2063 7265 6174 6520  ed is to create 
+00000a60: 6120 4648 4952 5374 6172 7465 7220 616e  a FHIRStarter an
+00000a70: 6420 610a 4648 4952 5072 6f76 6964 6572  d a.FHIRProvider
+00000a80: 2069 6e73 7461 6e63 652c 2072 6567 6973   instance, regis
+00000a90: 7465 7220 6120 4648 4952 2069 6e74 6572  ter a FHIR inter
+00000aa0: 6163 7469 6f6e 2077 6974 6820 7468 6520  action with the 
+00000ab0: 7072 6f76 6964 6572 2c20 6164 6420 7468  provider, add th
+00000ac0: 6520 7072 6f76 6964 6572 2074 6f20 7468  e provider to th
+00000ad0: 650a 4648 4952 5374 6172 7465 7220 696e  e.FHIRStarter in
+00000ae0: 7374 616e 6365 2c20 616e 6420 7061 7373  stance, and pass
+00000af0: 2074 6865 2046 4849 5253 7461 7274 6572   the FHIRStarter
+00000b00: 2069 6e73 7461 6e63 6520 746f 2061 6e20   instance to an 
+00000b10: 4153 4749 2073 6572 7665 722e 0a0a 2323  ASGI server...##
+00000b20: 2055 7361 6765 0a0a 2323 2320 4375 7272   Usage..### Curr
+00000b30: 656e 746c 792d 7375 7070 6f72 7465 6420  ently-supported 
+00000b40: 6675 6e63 7469 6f6e 616c 6974 790a 0a46  functionality..F
+00000b50: 4849 5253 7461 7274 6572 2073 7570 706f  HIRStarter suppo
+00000b60: 7274 7320 6372 6561 7465 2c20 7265 6164  rts create, read
+00000b70: 2c20 7365 6172 6368 2d74 7970 652c 2061  , search-type, a
+00000b80: 6e64 2075 7064 6174 6520 656e 6470 6f69  nd update endpoi
+00000b90: 6e74 7320 6163 726f 7373 2061 6c6c 2046  nts across all F
+00000ba0: 4849 5220 7265 736f 7572 6365 0a74 7970  HIR resource.typ
+00000bb0: 6573 2c20 616e 6420 7769 6c6c 2061 7574  es, and will aut
+00000bc0: 6f6d 6174 6963 616c 6c79 2067 656e 6572  omatically gener
+00000bd0: 6174 6520 7468 6520 602f 6d65 7461 6461  ate the `/metada
+00000be0: 7461 6020 6361 7061 6269 6c69 7469 6573  ta` capabilities
+00000bf0: 2073 7461 7465 6d65 6e74 2065 6e64 706f   statement endpo
+00000c00: 696e 742e 0a0a 4861 6e64 6c65 7273 2063  int...Handlers c
+00000c10: 616e 2062 6520 7772 6974 7465 6e20 6173  an be written as
+00000c20: 2063 6f72 6f75 7469 6e65 7320 7769 7468   coroutines with
+00000c30: 2060 6173 796e 632f 6177 6169 7460 2073   `async/await` s
+00000c40: 796e 7461 782c 206f 7220 6173 2070 6c61  yntax, or as pla
+00000c50: 696e 2066 756e 6374 696f 6e73 2e20 4661  in functions. Fa
+00000c60: 7374 4150 490a 7375 7070 6f72 7473 2062  stAPI.supports b
+00000c70: 6f74 682c 2061 7320 646f 6573 2046 4849  oth, as does FHI
+00000c80: 5253 7461 7274 6572 2e0a 0a23 2323 2043  RStarter...### C
+00000c90: 6f6e 6669 6775 7261 7469 6f6e 2066 6f72  onfiguration for
+00000ca0: 2073 7065 6369 6669 6320 4648 4952 2073   specific FHIR s
+00000cb0: 6571 7565 6e63 6573 0a0a 4648 4952 5374  equences..FHIRSt
+00000cc0: 6172 7465 7220 7769 6c6c 2077 6f72 6b20  arter will work 
+00000cd0: 6f75 7420 6f66 2074 6865 2062 6f78 2061  out of the box a
+00000ce0: 7320 616e 2052 3520 7365 7276 6572 2e20  s an R5 server. 
+00000cf0: 4966 2061 2064 6966 6665 7265 6e74 2073  If a different s
+00000d00: 6571 7565 6e63 6520 6973 2064 6573 6972  equence is desir
+00000d10: 6564 2c20 6974 206d 7573 7420 6265 0a73  ed, it must be.s
+00000d20: 7065 6369 6669 6564 2077 6974 6820 616e  pecified with an
+00000d30: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
+00000d40: 6961 626c 653a 0a0a 6060 6073 6865 6c6c  iable:..```shell
+00000d50: 0a46 4849 525f 5345 5155 454e 4345 3d22  .FHIR_SEQUENCE="
+00000d60: 5234 4222 0a60 6060 0a0a 5468 6520 6c61  R4B".```..The la
+00000d70: 7465 7374 2076 6572 7369 6f6e 206f 6620  test version of 
+00000d80: 7468 6520 5b46 4849 5220 5265 736f 7572  the [FHIR Resour
+00000d90: 6365 735d 2868 7474 7073 3a2f 2f70 7970  ces](https://pyp
+00000da0: 692e 6f72 672f 7072 6f6a 6563 742f 6668  i.org/project/fh
+00000db0: 6972 2e72 6573 6f75 7263 6573 2f29 2070  ir.resources/) p
+00000dc0: 6163 6b61 6765 206f 6e6c 790a 7375 7070  ackage only.supp
+00000dd0: 6f72 7473 2046 4849 5220 5354 5533 2c20  orts FHIR STU3, 
+00000de0: 5234 422c 2061 6e64 2052 352e 2046 4849  R4B, and R5. FHI
+00000df0: 5220 5234 2069 7320 7375 7070 6f72 7465  R R4 is supporte
+00000e00: 6420 6279 2061 6e20 6561 726c 6965 7220  d by an earlier 
+00000e10: 7665 7273 696f 6e2e 2042 6563 6175 7365  version. Because
+00000e20: 206f 6620 7468 6973 2c20 6966 2061 0a64   of this, if a.d
+00000e30: 6576 656c 6f70 6572 2064 6573 6972 6573  eveloper desires
+00000e40: 2074 6f20 7573 6520 4648 4952 2052 342c   to use FHIR R4,
+00000e50: 2074 6865 6e20 7468 6520 6465 7665 6c6f   then the develo
+00000e60: 7065 7220 6d75 7374 2070 696e 2076 6572  per must pin ver
+00000e70: 7369 6f6e 202a 2a36 2e34 2e30 2a2a 206f  sion **6.4.0** o
+00000e80: 6620 6668 6972 2e72 6573 6f75 7263 6573  f fhir.resources
+00000e90: 2069 6e0a 7468 6569 7220 7072 6f6a 6563   in.their projec
+00000ea0: 742e 2046 4849 5253 7461 7274 6572 2077  t. FHIRStarter w
+00000eb0: 696c 6c20 6368 6563 6b20 7468 6520 7665  ill check the ve
+00000ec0: 7273 696f 6e20 6f66 2066 6869 722e 7265  rsion of fhir.re
+00000ed0: 736f 7572 6365 7320 6167 6169 6e73 7420  sources against 
+00000ee0: 7468 6520 7370 6563 6966 6965 6420 4648  the specified FH
+00000ef0: 4952 0a76 6572 7369 6f6e 2069 6e20 7468  IR.version in th
+00000f00: 6520 656e 7669 726f 6e6d 656e 7420 7661  e environment va
+00000f10: 7269 6162 6c65 2074 6f20 656e 7375 7265  riable to ensure
+00000f20: 2074 6861 7420 7468 6579 2061 7265 2063   that they are c
+00000f30: 6f6d 7061 7469 626c 652e 0a0a 4d6f 6465  ompatible...Mode
+00000f40: 6c20 696d 706f 7274 7320 6172 6520 616c  l imports are al
+00000f50: 736f 2061 6666 6563 7465 6420 6279 2077  so affected by w
+00000f60: 6869 6368 2076 6572 7369 6f6e 206f 6620  hich version of 
+00000f70: 6668 6972 2e72 6573 6f75 7263 6573 2069  fhir.resources i
+00000f80: 7320 696e 7374 616c 6c65 642e 2046 6f72  s installed. For
+00000f90: 2053 5455 3320 616e 6420 5234 422c 0a6d   STU3 and R4B,.m
+00000fa0: 6f64 656c 2069 6d70 6f72 7473 2077 696c  odel imports wil
+00000fb0: 6c20 6c6f 6f6b 206c 696b 6520 7468 6973  l look like this
+00000fc0: 3a0a 0a60 6060 7079 7468 6f6e 0a66 726f  :..```python.fro
+00000fd0: 6d20 6668 6972 2e72 6573 6f75 7263 6573  m fhir.resources
+00000fe0: 2e53 5455 332e 7061 7469 656e 7420 696d  .STU3.patient im
+00000ff0: 706f 7274 2050 6174 6965 6e74 0a60 6060  port Patient.```
+00001000: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00001010: 6668 6972 2e72 6573 6f75 7263 6573 2e52  fhir.resources.R
+00001020: 3442 2e70 6174 6965 6e74 2069 6d70 6f72  4B.patient impor
+00001030: 7420 5061 7469 656e 740a 6060 600a 0a46  t Patient.```..F
+00001040: 6f72 2052 3420 616e 6420 5235 2c20 6d6f  or R4 and R5, mo
+00001050: 6465 6c20 696d 706f 7274 7320 7769 6c6c  del imports will
+00001060: 206c 6f6f 6b20 6c69 6b65 2074 6869 733a   look like this:
+00001070: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00001080: 2066 6869 722e 7265 736f 7572 6365 732e   fhir.resources.
+00001090: 7061 7469 656e 7420 696d 706f 7274 2050  patient import P
+000010a0: 6174 6965 6e74 0a60 6060 0a0a 2323 2320  atient.```..### 
+000010b0: 4578 616d 706c 650a 0a41 2064 6574 6169  Example..A detai
+000010c0: 6c65 6420 6578 616d 706c 6520 6973 2061  led example is a
+000010d0: 7661 696c 6162 6c65 2068 6572 653a 205b  vailable here: [
+000010e0: 6578 616d 706c 652e 7079 5d28 6874 7470  example.py](http
+000010f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+00001100: 616e 7661 732d 6d65 6469 6361 6c2f 6668  anvas-medical/fh
+00001110: 6972 7374 6172 7465 722f 626c 6f62 2f6d  irstarter/blob/m
+00001120: 6169 6e2f 6668 6972 7374 6172 7465 722f  ain/fhirstarter/
+00001130: 7363 7269 7074 732f 6578 616d 706c 652e  scripts/example.
+00001140: 7079 292e 0a0a 6060 6070 7974 686f 6e0a  py)...```python.
+00001150: 696d 706f 7274 2075 7669 636f 726e 0a66  import uvicorn.f
+00001160: 726f 6d20 6668 6972 2e72 6573 6f75 7263  rom fhir.resourc
+00001170: 6573 2e66 6869 7274 7970 6573 2069 6d70  es.fhirtypes imp
+00001180: 6f72 7420 4964 0a66 726f 6d20 6668 6972  ort Id.from fhir
+00001190: 2e72 6573 6f75 7263 6573 2e70 6174 6965  .resources.patie
+000011a0: 6e74 2069 6d70 6f72 7420 5061 7469 656e  nt import Patien
+000011b0: 740a 0a66 726f 6d20 6668 6972 7374 6172  t..from fhirstar
+000011c0: 7465 7220 696d 706f 7274 2046 4849 5250  ter import FHIRP
+000011d0: 726f 7669 6465 722c 2046 4849 5253 7461  rovider, FHIRSta
+000011e0: 7274 6572 2c20 496e 7465 7261 6374 696f  rter, Interactio
+000011f0: 6e43 6f6e 7465 7874 0a66 726f 6d20 6668  nContext.from fh
+00001200: 6972 7374 6172 7465 722e 6578 6365 7074  irstarter.except
+00001210: 696f 6e73 2069 6d70 6f72 7420 4648 4952  ions import FHIR
+00001220: 5265 736f 7572 6365 4e6f 7446 6f75 6e64  ResourceNotFound
+00001230: 4572 726f 720a 0a23 2043 7265 6174 6520  Error..# Create 
+00001240: 7468 6520 6170 700a 6170 7020 3d20 4648  the app.app = FH
+00001250: 4952 5374 6172 7465 7228 290a 0a23 2043  IRStarter()..# C
+00001260: 7265 6174 6520 6120 7072 6f76 6964 6572  reate a provider
+00001270: 0a70 726f 7669 6465 7220 3d20 4648 4952  .provider = FHIR
+00001280: 5072 6f76 6964 6572 2829 0a0a 0a23 2052  Provider()...# R
+00001290: 6567 6973 7465 7220 7468 6520 7061 7469  egister the pati
+000012a0: 656e 7420 7265 6164 2046 4849 5220 696e  ent read FHIR in
+000012b0: 7465 7261 6374 696f 6e20 7769 7468 2074  teraction with t
+000012c0: 6865 2070 726f 7669 6465 720a 4070 726f  he provider.@pro
+000012d0: 7669 6465 722e 7265 6164 2850 6174 6965  vider.read(Patie
+000012e0: 6e74 290a 6173 796e 6320 6465 6620 7061  nt).async def pa
+000012f0: 7469 656e 745f 7265 6164 2863 6f6e 7465  tient_read(conte
+00001300: 7874 3a20 496e 7465 7261 6374 696f 6e43  xt: InteractionC
+00001310: 6f6e 7465 7874 2c20 6964 5f3a 2049 6429  ontext, id_: Id)
+00001320: 202d 3e20 5061 7469 656e 743a 0a20 2020   -> Patient:.   
+00001330: 2023 2047 6574 2074 6865 2070 6174 6965   # Get the patie
+00001340: 6e74 2066 726f 6d20 7468 6520 6461 7461  nt from the data
+00001350: 6261 7365 0a20 2020 2070 6174 6965 6e74  base.    patient
+00001360: 203d 202e 2e2e 0a0a 2020 2020 6966 206e   = .....    if n
+00001370: 6f74 2070 6174 6965 6e74 3a0a 2020 2020  ot patient:.    
+00001380: 2020 2020 7261 6973 6520 4648 4952 5265      raise FHIRRe
+00001390: 736f 7572 6365 4e6f 7446 6f75 6e64 4572  sourceNotFoundEr
+000013a0: 726f 720a 0a20 2020 2072 6574 7572 6e20  ror..    return 
+000013b0: 5061 7469 656e 7428 0a20 2020 2020 2020  Patient(.       
+000013c0: 202a 2a7b 0a20 2020 2020 2020 2020 2020   **{.           
+000013d0: 2023 204d 6170 2070 6174 6965 6e74 2066   # Map patient f
+000013e0: 726f 6d20 6461 7461 6261 7365 2074 6f20  rom database to 
+000013f0: 4648 4952 2050 6174 6965 6e74 2073 7472  FHIR Patient str
+00001400: 7563 7475 7265 0a20 2020 2020 2020 207d  ucture.        }
+00001410: 0a20 2020 2029 0a0a 0a23 2041 6464 2074  .    )...# Add t
+00001420: 6865 2070 726f 7669 6465 7220 746f 2074  he provider to t
+00001430: 6865 2061 7070 0a61 7070 2e61 6464 5f70  he app.app.add_p
+00001440: 726f 7669 6465 7273 2870 726f 7669 6465  roviders(provide
+00001450: 7229 0a0a 0a69 6620 5f5f 6e61 6d65 5f5f  r)...if __name__
+00001460: 203d 3d20 225f 5f6d 6169 6e5f 5f22 3a0a   == "__main__":.
+00001470: 2020 2020 2320 5374 6172 7420 7468 6520      # Start the 
+00001480: 7365 7276 6572 0a20 2020 2075 7669 636f  server.    uvico
+00001490: 726e 2e72 756e 2861 7070 290a 6060 600a  rn.run(app).```.
+000014a0: 0a23 2323 2043 7573 746f 6d20 7365 6172  .### Custom sear
+000014b0: 6368 2070 6172 616d 6574 6572 730a 0a43  ch parameters..C
+000014c0: 7573 746f 6d20 7365 6172 6368 2070 6172  ustom search par
+000014d0: 616d 6574 6572 7320 6361 6e20 6265 2064  ameters can be d
+000014e0: 6566 696e 6564 2069 6e20 6120 636f 6e66  efined in a conf
+000014f0: 6967 7572 6174 696f 6e20 6669 6c65 2074  iguration file t
+00001500: 6861 7420 6361 6e20 6265 2070 6173 7365  hat can be passe
+00001510: 6420 746f 2074 6865 2061 7070 206f 6e0a  d to the app on.
+00001520: 6372 6561 7469 6f6e 2e0a 0a60 6060 746f  creation...```to
+00001530: 6d6c 0a5b 7365 6172 6368 2d70 6172 616d  ml.[search-param
+00001540: 6574 6572 732e 5061 7469 656e 742e 6e69  eters.Patient.ni
+00001550: 636b 6e61 6d65 5d0a 7479 7065 203d 2022  ckname].type = "
+00001560: 7374 7269 6e67 220a 6465 7363 7269 7074  string".descript
+00001570: 696f 6e20 3d20 224e 6963 6b6e 616d 6522  ion = "Nickname"
+00001580: 0a75 7269 203d 2022 6874 7470 733a 2f2f  .uri = "https://
+00001590: 686f 7374 6e61 6d65 2f6e 6963 6b6e 616d  hostname/nicknam
+000015a0: 6522 0a69 6e63 6c75 6465 2d69 6e2d 6361  e".include-in-ca
+000015b0: 7061 6269 6c69 7479 2d73 7461 7465 6d65  pability-stateme
+000015c0: 6e74 203d 2074 7275 650a 6060 600a 0a41  nt = true.```..A
+000015d0: 6464 696e 6720 6120 6375 7374 6f6d 2073  dding a custom s
+000015e0: 6561 7263 6820 7061 7261 6d65 7465 7220  earch parameter 
+000015f0: 7669 6120 636f 6e66 6967 7572 6174 696f  via configuratio
+00001600: 6e20 616c 6c6f 7773 2074 6869 7320 6e61  n allows this na
+00001610: 6d65 2074 6f20 6265 2075 7365 6420 6173  me to be used as
+00001620: 2061 6e20 6172 6775 6d65 6e74 2077 6865   an argument whe
+00001630: 6e0a 6465 6669 6e69 6e67 2061 2073 6561  n.defining a sea
+00001640: 7263 682d 7479 7065 2069 6e74 6572 6163  rch-type interac
+00001650: 7469 6f6e 2068 616e 646c 6572 2061 6e64  tion handler and
+00001660: 2061 6c73 6f20 6164 6473 2074 6869 7320   also adds this 
+00001670: 7365 6172 6368 2070 6172 616d 6574 6572  search parameter
+00001680: 2074 6f20 7468 6520 4150 490a 646f 6375   to the API.docu
+00001690: 6d65 6e74 6174 696f 6e20 666f 7220 7468  mentation for th
+000016a0: 6520 7365 6172 6368 2065 6e64 706f 696e  e search endpoin
+000016b0: 742e 0a0a 2323 2320 4361 7061 6269 6c69  t...### Capabili
+000016c0: 7479 2073 7461 7465 6d65 6e74 0a0a 4974  ty statement..It
+000016d0: 2069 7320 706f 7373 6962 6c65 2074 6f20   is possible to 
+000016e0: 6375 7374 6f6d 697a 6520 7468 6520 6361  customize the ca
+000016f0: 7061 6269 6c69 7479 2073 7461 7465 6d65  pability stateme
+00001700: 6e74 2062 7920 7365 7474 696e 6720 6120  nt by setting a 
+00001710: 6361 7061 6269 6c69 7479 2073 7461 7465  capability state
+00001720: 6d65 6e74 206d 6f64 6966 6965 723a 0a0a  ment modifier:..
+00001730: 6060 6070 7974 686f 6e0a 6465 6620 616d  ```python.def am
+00001740: 656e 645f 6361 7061 6269 6c69 7479 5f73  end_capability_s
+00001750: 7461 7465 6d65 6e74 280a 2020 2020 6361  tatement(.    ca
+00001760: 7061 6269 6c69 7479 5f73 7461 7465 6d65  pability_stateme
+00001770: 6e74 3a20 4d75 7461 626c 654d 6170 7069  nt: MutableMappi
+00001780: 6e67 5b73 7472 2c20 416e 795d 2c20 7265  ng[str, Any], re
+00001790: 7175 6573 743a 2052 6571 7565 7374 2c20  quest: Request, 
+000017a0: 7265 7370 6f6e 7365 3a20 5265 7370 6f6e  response: Respon
+000017b0: 7365 0a29 202d 3e20 4d75 7461 626c 654d  se.) -> MutableM
+000017c0: 6170 7069 6e67 5b73 7472 2c20 416e 795d  apping[str, Any]
+000017d0: 3a0a 2020 2020 6361 7061 6269 6c69 7479  :.    capability
+000017e0: 5f73 7461 7465 6d65 6e74 5b22 7075 626c  _statement["publ
+000017f0: 6973 6865 7222 5d20 3d20 2243 616e 7661  isher"] = "Canva
+00001800: 7320 4d65 6469 6361 6c22 0a20 2020 2072  s Medical".    r
+00001810: 6574 7572 6e20 6361 7061 6269 6c69 7479  eturn capability
+00001820: 5f73 7461 7465 6d65 6e74 0a0a 6170 702e  _statement..app.
+00001830: 7365 745f 6361 7061 6269 6c69 7479 5f73  set_capability_s
+00001840: 7461 7465 6d65 6e74 5f6d 6f64 6966 6965  tatement_modifie
+00001850: 7228 616d 656e 645f 6361 7061 6269 6c69  r(amend_capabili
+00001860: 7479 5f73 7461 7465 6d65 6e74 290a 6060  ty_statement).``
+00001870: 600a 0a23 2323 2046 6173 7441 5049 2064  `..### FastAPI d
+00001880: 6570 656e 6465 6e63 7920 696e 6a65 6374  ependency inject
+00001890: 696f 6e0a 0a46 6173 7441 5049 2773 2064  ion..FastAPI's d
+000018a0: 6570 656e 6465 6e63 7920 696e 6a65 6374  ependency inject
+000018b0: 696f 6e20 6973 2065 7870 6f73 6564 2061  ion is exposed a
+000018c0: 7420 7661 7269 6f75 7320 6c65 7665 6c73  t various levels
+000018d0: 3a0a 0a2a 202a 2a61 7070 6c69 6361 7469  :..* **applicati
+000018e0: 6f6e 2a2a 3a20 7468 6520 605f 5f69 6e69  on**: the `__ini
+000018f0: 745f 5f60 206d 6574 686f 6420 6f6e 2074  t__` method on t
+00001900: 6865 2046 4849 5253 7461 7274 6572 2063  he FHIRStarter c
+00001910: 6c61 7373 0a2a 202a 2a70 726f 7669 6465  lass.* **provide
+00001920: 722a 2a3a 2074 6865 2060 5f5f 696e 6974  r**: the `__init
+00001930: 5f5f 6020 6d65 7468 6f64 206f 6e20 7468  __` method on th
+00001940: 6520 4648 4952 5072 6f76 6964 6572 2063  e FHIRProvider c
+00001950: 6c61 7373 0a2a 202a 2a68 616e 646c 6572  lass.* **handler
+00001960: 2a2a 3a20 7468 6520 6063 7265 6174 6560  **: the `create`
+00001970: 2c20 6072 6561 6460 2c20 6073 6561 7263  , `read`, `searc
+00001980: 685f 7479 7065 602c 206f 7220 6075 7064  h_type`, or `upd
+00001990: 6174 6560 2064 6563 6f72 6174 6f72 2075  ate` decorator u
+000019a0: 7365 6420 746f 2061 6464 2061 2068 616e  sed to add a han
+000019b0: 646c 6572 2074 6f20 6120 7072 6f76 6964  dler to a provid
+000019c0: 6572 0a0a 4465 7065 6e64 656e 6369 6573  er..Dependencies
+000019d0: 2073 7065 6369 6669 6564 2061 7420 7468   specified at th
+000019e0: 6520 6170 706c 6963 6174 696f 6e20 6c65  e application le
+000019f0: 7665 6c20 7769 6c6c 2062 6520 696e 6a65  vel will be inje
+00001a00: 6374 6564 2069 6e74 6f20 616c 6c20 726f  cted into all ro
+00001a10: 7574 6573 2069 6e20 7468 6520 6170 706c  utes in the appl
+00001a20: 6963 6174 696f 6e2e 0a0a 4465 7065 6e64  ication...Depend
+00001a30: 656e 6369 6573 2073 7065 6369 6669 6564  encies specified
+00001a40: 2061 7420 7468 6520 7072 6f76 6964 6572   at the provider
+00001a50: 206c 6576 656c 2077 696c 6c20 6265 2069   level will be i
+00001a60: 6e6a 6563 7465 6420 696e 746f 2061 6c6c  njected into all
+00001a70: 2072 6f75 7465 7320 7468 6174 2061 7265   routes that are
+00001a80: 2061 6464 6564 2074 6f0a 7468 6520 6170   added to.the ap
+00001a90: 706c 6963 6174 696f 6e20 6672 6f6d 2074  plication from t
+00001aa0: 6861 7420 7370 6563 6966 6963 2070 726f  hat specific pro
+00001ab0: 7669 6465 722e 0a0a 4465 7065 6e64 656e  vider...Dependen
+00001ac0: 6369 6573 2073 7065 6369 6669 6564 2061  cies specified a
+00001ad0: 7420 7468 6520 6861 6e64 6c65 7220 6c65  t the handler le
+00001ae0: 7665 6c20 6f6e 6c79 2061 7070 6c79 2074  vel only apply t
+00001af0: 6f20 7468 6174 2073 7065 6369 6669 6320  o that specific 
+00001b00: 4648 4952 2069 6e74 6572 6163 7469 6f6e  FHIR interaction
+00001b10: 2e0a                                     ..
```

### Comparing `fhirstarter-0.13.9/fhirstarter/exceptions.py` & `fhirstarter-1.0.0/fhirstarter/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 containing an OperationOutcome and an HTTP status code.
 """
 
 from abc import ABC, abstractmethod
 
 from fastapi import Request, status
 from fastapi.exceptions import HTTPException
-from fhir.resources.operationoutcome import OperationOutcome
 
+from .resources import OperationOutcome
 from .utils import make_operation_outcome, parse_fhir_request
 
 
 class FHIRException(HTTPException, ABC):
     """
     Abstract base class for all FHIR exceptions.
```

### Comparing `fhirstarter-0.13.9/fhirstarter/fhirstarter.py` & `fhirstarter-1.0.0/fhirstarter/fhirstarter.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,18 @@
 from typing import Any, TypeAlias, cast
 from urllib.parse import parse_qs, urlencode
 from zoneinfo import ZoneInfo
 
 import uvloop
 from fastapi import FastAPI, HTTPException, Request, Response, status
 from fastapi.exceptions import RequestValidationError
-from fhir.resources.capabilitystatement import CapabilityStatement
-from fhir.resources.operationoutcome import OperationOutcome
 from pydantic.error_wrappers import display_errors
 
 from .exceptions import FHIRException
+from .fhir_specification import FHIR_SEQUENCE, FHIR_VERSION
 from .fhir_specification.utils import (
     create_bundle_example,
     is_resource_type,
     load_example,
     make_operation_outcome_example,
 )
 from .functions import (
@@ -34,14 +33,15 @@
     make_create_function,
     make_read_function,
     make_search_type_function,
     make_update_function,
 )
 from .interactions import ResourceType, TypeInteraction
 from .providers import FHIRProvider
+from .resources import CapabilityStatement, OperationOutcome
 from .search_parameters import (
     SearchParameters,
     search_parameter_sort_key,
     supported_search_parameters,
     var_name_to_qp_name,
 )
 from .utils import (
@@ -314,24 +314,28 @@
                 )
             resources.append(resource)
 
         capability_statement = {
             "status": "active",
             "date": self._created,
             "kind": "instance",
-            "fhirVersion": "4.0.1",
+            "fhirVersion": FHIR_VERSION,
+            "acceptUnknown": "no",
             "format": ["json"],
             "rest": [
                 {
                     "mode": "server",
                     "resource": resources,
                 }
             ],
         }
 
+        if FHIR_SEQUENCE != "STU3":
+            del capability_statement["acceptUnknown"]
+
         if self._capability_statement_modifier:
             capability_statement = self._capability_statement_modifier(
                 capability_statement, request, response
             )
 
         return CapabilityStatement(**capability_statement)
 
@@ -346,45 +350,30 @@
         This method is slightly hacky because it directly modifies the OpenAPI schema, however it
         does make the generated documentation look nicer.
 
         Because it directly modifies the OpenAPI schema, it is vulnerable to breakage from updates
         to FastAPI. This is not a significant vulnerability because the core server functionality
         will still work (i.e. this is just documentation).
         """
-        # TODO: It may be necessary to rethink some of the things that this function removes. For
-        #  example, if someone wants to add non-FHIR endpoints to their API, then maybe some of
-        #  these schemas shouldn't be removed. Also, for cases where paths or schemas are modified,
-        #  there should be a way to more precisely target items that are FHIR-related.
         if self.openapi_schema:
             return self.openapi_schema
 
         openapi_schema = super().openapi()
 
-        # Remove default FAstAPI validation errors, since FHIRStarter will always return operation
-        # outcomes
-        openapi_schema["components"]["schemas"].pop("HTTPValidationError", None)
-        openapi_schema["components"]["schemas"].pop("ValidationError", None)
-
-        # Add schema example for different operation outcomes
+        # Make schema examples for different operation outcomes
+        operation_outcome_examples = {}
         for status_code, code, details_text in (
-            (400, "invalid", "Bad Request"),
-            (401, "unknown", "Authentication failed"),
-            (403, "forbidden", "Authorization failed"),
-            (404, "not-found", "Resource Not Found"),
-            (422, "processing", "Unprocessable Entity"),
-            (500, "exception", "Internal Server Error"),
+            ("400", "invalid", "Bad Request"),
+            ("401", "unknown", "Authentication failed"),
+            ("403", "forbidden", "Authorization failed"),
+            ("404", "not-found", "Resource Not Found"),
+            ("422", "processing", "Unprocessable Entity"),
+            ("500", "exception", "Internal Server Error"),
         ):
-            title = f"OperationOutcome {status_code}"
-            openapi_schema["components"]["schemas"][title] = deepcopy(
-                openapi_schema["components"]["schemas"]["OperationOutcome"]
-            )
-            openapi_schema["components"]["schemas"][title]["title"] = title
-            openapi_schema["components"]["schemas"][title][
-                "example"
-            ] = make_operation_outcome_example(
+            operation_outcome_examples[status_code] = make_operation_outcome_example(
                 severity="error", code=code, details_text=details_text
             )
 
         # For each schema (except for Bundle and OperationOutcome), provide an actual FHIR example
         # response unless an example exists on the actual model
         for schema_name, schema in openapi_schema["components"]["schemas"].items():
             resource_type = schema["properties"].get("resource_type", {}).get("const")
@@ -403,15 +392,15 @@
             # Inline the schemas generated for search by POST. These schemas are only used in one
             # place, so they don't need to exist in the schemas section.
             if match := re.fullmatch("/(.*)/_search", path_name):
                 resource_type = match.group(1)
                 path["post"]["requestBody"]["content"][
                     "application/x-www-form-urlencoded"
                 ]["schema"] = openapi_schema["components"]["schemas"].pop(
-                    f"Body_fhirstarter_type_search_post_{resource_type}"
+                    f"Body_fhirstarter_type_search-type_post_{resource_type}"
                 )
 
             # Iterate over all operations for a given path
             for operation_name, operation in path.items():
                 # For each possible response (i.e. status code), remove the default FastAPI response
                 # schema
                 responses = operation["responses"]
@@ -424,51 +413,53 @@
                         .get("$ref")
                         == "#/components/schemas/HTTPValidationError"
                     ):
                         responses.pop(status_code)
 
                 # For each response, change all instances of application/json to
                 # application/fhir+json
-                # Iterate over the responses
                 for status_code, response in responses.items():
-                    # Remove the response for "application/json"
+                    # Move the response for "application/json" to "application/fhir+json"
                     schema = response["content"].pop("application/json", None)
+                    if schema:
+                        response["content"]["application/fhir+json"] = schema
 
                     # Add specialized OperationOutcome responses if available for the status code
-                    if (
-                        f"OperationOutcome {status_code}"
-                        in openapi_schema["components"]["schemas"]
+                    if operation_outcome_example := operation_outcome_examples.get(
+                        status_code
                     ):
-                        response["content"]["application/fhir+json"] = openapi_schema[
-                            "components"
-                        ]["schemas"][f"OperationOutcome {status_code}"]
-                    elif schema:
-                        # If there was a response originally, add it back as the response for
-                        # application/fhir+json
-                        response["content"]["application/fhir+json"] = schema
+                        response["content"]["application/fhir+json"][
+                            "example"
+                        ] = operation_outcome_example
 
                 # For search operations, provide a bundle example that contains the correct resource
                 # type
                 if "|" in (
                     operation_id := operation["operationId"]
                 ) and operation_id.startswith("fhirstarter|"):
                     _, _, interaction_type, *rest = operation_id.split("|")
-                    if interaction_type == "search":
+                    if interaction_type == "search-type":
                         resource_type = rest[1]
 
-                        if is_resource_type(resource_type):
-                            example = load_example(resource_type)
-                        else:
-                            try:
-                                example = self._capabilities[resource_type][
-                                    "search-type"
-                                ].resource_type.Config.schema_extra["example"]
-                            except (AttributeError, KeyError):
+                        # Get the example for the resource. If a custom example is defined, it will
+                        # be used, otherwise an example will be loaded from the FHIR specification.
+                        try:
+                            example = self._capabilities[resource_type][
+                                "search-type"
+                            ].resource_type.Config.schema_extra["example"]
+                        except (AttributeError, KeyError):
+                            example = None
+                        if not example:
+                            if is_resource_type(resource_type):
+                                example = load_example(resource_type)
+                            else:
                                 example = {"resourceType": resource_type}
 
+                        # For successful responses, copy the schema, and create and set a bundle
+                        # example that includes the example resource
                         operation["responses"]["200"]["content"][
                             "application/fhir+json"
                         ]["schema"] = deepcopy(
                             openapi_schema["components"]["schemas"]["Bundle"]
                         )
                         operation["responses"]["200"]["content"][
                             "application/fhir+json"
```

### Comparing `fhirstarter-0.13.9/fhirstarter/functions.py` & `fhirstarter-1.0.0/fhirstarter/functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,35 +7,43 @@
 chain.
 
 The search use case is slightly more complicated. Because each FHIR resource type has a different
 set of search parameters (i.e. query parameters), the approach used for the create, read, and update
 use cases to create the callables does not work. Instead, a function that takes arbitrary kwargs is
 created, and the function signature is modified afterward to provide the information needed by
 FastAPI for documentation purposes: variable name, annotation, and default value.
+
+These functions can create FastAPI path operation functions for both async and non-async handlers,
+though not elegantly. Unfortunately the code has to be duplicated, and maintainers will need to be
+cognizant that changes made to these generated path operation functions must be applied in two
+places.
 """
 
 import keyword
 from collections.abc import Callable, Coroutine
-from inspect import Parameter, signature
+from inspect import Parameter, iscoroutinefunction, signature
 from typing import cast
 
 from fastapi import Body, Form, Path, Query, Request, Response
-from fhir.resources.fhirtypes import Id
-from fhir.resources.resource import Resource
 
 from .exceptions import FHIRBadRequestError
 from .interactions import (
+    CreateInteractionAsyncHandler,
     CreateInteractionHandler,
     InteractionContext,
+    ReadInteractionAsyncHandler,
     ReadInteractionHandler,
     ResourceType,
+    SearchTypeInteractionAsyncHandler,
     SearchTypeInteractionHandler,
     TypeInteraction,
+    UpdateInteractionAsyncHandler,
     UpdateInteractionHandler,
 )
+from .resources import Bundle, Id, Resource
 from .search_parameters import (
     search_parameter_sort_key,
     supported_search_parameters,
     var_name_to_qp_name,
 )
 from .utils import FormatParameters, format_response
 
@@ -46,215 +54,355 @@
     "Ask for a pretty printed response for human convenience"
 )
 
 FORMAT_QP = Query(None, description=_FORMAT_PARAMETER_DESCRIPTION)
 PRETTY_QP = Query(None, description=_PRETTY_PARAMETER_DESCRIPTION)
 
 
+# Note: I'm not currently aware of a better way do support both async and non-async handlers than
+#       branching based on the result of the iscoroutinefunction function and duplicating most of
+#       the code. If there is a better way to do this, I will refactor later.
+
+
 def make_create_function(
     interaction: TypeInteraction[ResourceType],
 ) -> Callable[
     [Request, Response, str, str, ResourceType],
-    Coroutine[None, None, ResourceType | Response | None],
+    Coroutine[None, None, ResourceType | Response | None]
+    | ResourceType
+    | Response
+    | None,
 ]:
     """Make a function suitable for creation of a FHIR create API route."""
     resource_type_str = interaction.resource_type.get_resource_type()
 
-    async def create(
-        request: Request,
-        response: Response,
-        _format: str = FORMAT_QP,
-        _pretty: str = PRETTY_QP,
-        resource: ResourceType = Body(
-            None,
-            media_type="application/fhir+json",
-            alias=resource_type_str,
-        ),
-    ) -> ResourceType | Response | None:
-        """
-        Function for create interaction.
-
-        Calls the handler, and sets the Location header based on the Id of the created resource.
-        """
-        handler = cast(CreateInteractionHandler[ResourceType], interaction.handler)
-        result = await handler(InteractionContext(request, response), resource)  # type: ignore
-        id_, result_resource = _result_to_id_resource_tuple(result)
-
-        response.headers[
-            "Location"
-        ] = f"{request.base_url}{resource_type_str}/{id_}/_history/1"
-
-        return format_response(
-            resource=result_resource,
-            response=response,
-            format_parameters=FormatParameters.from_request(request),
-        )
+    if iscoroutinefunction(interaction.handler):
 
-    create.__annotations__ |= {
-        "resource": interaction.resource_type,
-    }
+        async def create_async(
+            request: Request,
+            response: Response,
+            _format: str = FORMAT_QP,
+            _pretty: str = PRETTY_QP,
+            resource: ResourceType = Body(
+                None,
+                media_type="application/fhir+json",
+                alias=resource_type_str,
+            ),
+        ) -> ResourceType | Response | None:
+            """
+            Function for create interaction.
+
+            Calls the handler, and sets the Location header based on the Id of the created resource.
+            """
+            handler = cast(
+                CreateInteractionAsyncHandler[ResourceType], interaction.handler
+            )
+            result = await handler(InteractionContext(request, response), resource)  # type: ignore
+            id_, result_resource = _result_to_id_resource_tuple(result)
 
-    return create
+            response.headers[
+                "Location"
+            ] = f"{request.base_url}{resource_type_str}/{id_}/_history/1"
+
+            return format_response(
+                resource=result_resource,
+                response=response,
+                format_parameters=FormatParameters.from_request(request),
+            )
+
+        create_async.__annotations__ |= {
+            "resource": interaction.resource_type,
+        }
+
+        return create_async
+    else:
+
+        def create(
+            request: Request,
+            response: Response,
+            _format: str = FORMAT_QP,
+            _pretty: str = PRETTY_QP,
+            resource: ResourceType = Body(
+                None, media_type="application/fhir+json", alias=resource_type_str
+            ),
+        ) -> ResourceType | Response | None:
+            """
+            Function for create interaction.
+
+            Calls the handler, and sets the Location header based on the Id of the created resource.
+            """
+            handler = cast(CreateInteractionHandler[ResourceType], interaction.handler)
+            result = handler(InteractionContext(request, response), resource)  # type: ignore
+            id_, result_resource = _result_to_id_resource_tuple(result)
+
+            response.headers[
+                "Location"
+            ] = f"{request.base_url}{resource_type_str}/{id_}/_history/1"
+
+            return format_response(
+                resource=result_resource,
+                response=response,
+                format_parameters=FormatParameters.from_request(request),
+            )
+
+        create.__annotations__ |= {
+            "resource": interaction.resource_type,
+        }
+
+        return create
 
 
 def make_read_function(
     interaction: TypeInteraction[ResourceType],
 ) -> Callable[
-    [Request, Response, Id, str, str], Coroutine[None, None, ResourceType | Response]
+    [Request, Response, Id, str, str],
+    Coroutine[None, None, ResourceType | Response] | ResourceType | Response,
 ]:
     """Make a function suitable for creation of a FHIR read API route."""
 
-    async def read(
-        request: Request,
-        response: Response,
-        id_: Id = Path(
-            None,
-            alias="id",
-            description=Resource.schema()["properties"]["id"]["title"],
-        ),
-        _format: str = FORMAT_QP,
-        _pretty: str = PRETTY_QP,
-    ) -> ResourceType | Response:
-        """Function for read interaction."""
-        handler = cast(ReadInteractionHandler[ResourceType], interaction.handler)
-        result_resource = await handler(InteractionContext(request, response), id_)  # type: ignore
-
-        return format_response(
-            resource=result_resource,
-            response=response,
-            format_parameters=FormatParameters.from_request(request),
-        )
+    if iscoroutinefunction(interaction.handler):
 
-    return read
+        async def read_async(
+            request: Request,
+            response: Response,
+            id_: Id = Path(
+                None,
+                alias="id",
+                description=Resource.schema()["properties"]["id"]["title"],
+            ),
+            _format: str = FORMAT_QP,
+            _pretty: str = PRETTY_QP,
+        ) -> ResourceType | Response:
+            """Function for read interaction."""
+            handler = cast(
+                ReadInteractionAsyncHandler[ResourceType], interaction.handler
+            )
+            result_resource = await handler(InteractionContext(request, response), id_)  # type: ignore
+
+            return format_response(
+                resource=result_resource,
+                response=response,
+                format_parameters=FormatParameters.from_request(request),
+            )
+
+        return read_async
+
+    else:
+
+        def read(
+            request: Request,
+            response: Response,
+            id_: Id = Path(
+                None,
+                alias="id",
+                description=Resource.schema()["properties"]["id"]["title"],
+            ),
+            _format: str = FORMAT_QP,
+            _pretty: str = PRETTY_QP,
+        ) -> ResourceType | Response:
+            """Function for read interaction."""
+            handler = cast(ReadInteractionHandler[ResourceType], interaction.handler)
+            result_resource = handler(InteractionContext(request, response), id_)  # type: ignore
+
+            return format_response(
+                resource=result_resource,
+                response=response,
+                format_parameters=FormatParameters.from_request(request),
+            )
+
+        return read
 
 
 # TODO: If possible, map FHIR primitives to correct type annotations for better validation
 def make_search_type_function(
     interaction: TypeInteraction[ResourceType],
     search_parameter_metadata: dict[str, dict[str, str]],
     post: bool,
 ) -> Callable[
-    [Request, Response, str, str], Coroutine[None, None, Resource | Response]
+    [Request, Response, str, str],
+    Coroutine[None, None, Bundle | Response] | Bundle | Response,
 ]:
     """
     Make a function suitable for creation of a FHIR search-type API route.
 
     Creation of a search-type function is more complex than creation of a create, read, or update
     function due to the variability of search parameters, support for custom search parameters, and
     due to the need to support GET and POST.
 
     Search parameter descriptions are pulled from the FHIR specification.
 
     After the function is created, the function signature is changed to account for what search
     parameters are supported by the developer-defined handler.
     """
-
     if post:
         format_annotation = Form(None, description=_FORMAT_PARAMETER_DESCRIPTION)
         pretty_annotation = Form(None, description=_PRETTY_PARAMETER_DESCRIPTION)
     else:
         format_annotation = FORMAT_QP
         pretty_annotation = PRETTY_QP
 
-    async def search_type(
-        request: Request,
-        response: Response,
-        *,
-        _format: str = format_annotation,
-        _pretty: str = pretty_annotation,
-        **kwargs: str,
-    ) -> Resource | Response:
-        """Function for search-type interaction."""
-        handler = cast(SearchTypeInteractionHandler, interaction.handler)
-        bundle = await handler(InteractionContext(request, response), **kwargs)  # type: ignore
-
-        return format_response(
-            resource=bundle,
-            response=response,
-            format_parameters=FormatParameters.from_request(request),
-        )
-
     search_parameters: tuple[Parameter, ...] = tuple(
         _make_search_parameter(
             name=search_parameter.name,
             description=search_parameter_metadata[
                 var_name_to_qp_name(search_parameter.name)
             ]["description"],
             post=post,
             multiple=search_parameter.multiple,
         )
         for search_parameter in supported_search_parameters(interaction.handler)
     )
 
-    sig = signature(search_type)
-    parameters: tuple[Parameter, ...] = tuple(sig.parameters.values())[:-1]
+    if iscoroutinefunction(interaction.handler):
 
-    sorted_search_parameters: list[Parameter] = sorted(
-        parameters + search_parameters,
-        key=lambda p: search_parameter_sort_key(
-            p.name, search_parameter_metadata, p.annotation
-        ),
-    )
+        async def search_type_async(
+            request: Request,
+            response: Response,
+            *,
+            _format: str = format_annotation,
+            _pretty: str = pretty_annotation,
+            **kwargs: str,
+        ) -> Bundle | Response:
+            """Function for search-type interaction."""
+            handler = cast(SearchTypeInteractionAsyncHandler, interaction.handler)
+            bundle = await handler(InteractionContext(request, response), **kwargs)  # type: ignore
+
+            return format_response(
+                resource=bundle,
+                response=response,
+                format_parameters=FormatParameters.from_request(request),
+            )
 
-    sig = sig.replace(parameters=sorted_search_parameters)
-    setattr(search_type, "__signature__", sig)
+        return _set_search_type_function_signature(
+            search_type_async, search_parameters, search_parameter_metadata
+        )
+
+    else:
+
+        def search_type(
+            request: Request,
+            response: Response,
+            *,
+            _format: str = format_annotation,
+            _pretty: str = pretty_annotation,
+            **kwargs: str,
+        ) -> Bundle | Response:
+            """Function for search-type interaction."""
+            handler = cast(SearchTypeInteractionHandler, interaction.handler)
+            bundle = handler(InteractionContext(request, response), **kwargs)  # type: ignore
+
+            return format_response(
+                resource=bundle,
+                response=response,
+                format_parameters=FormatParameters.from_request(request),
+            )
 
-    return search_type
+        return _set_search_type_function_signature(
+            search_type, search_parameters, search_parameter_metadata
+        )
 
 
 def make_update_function(
     interaction: TypeInteraction[ResourceType],
 ) -> Callable[
     [Request, Response, Id, str, str, ResourceType],
-    Coroutine[None, None, ResourceType | Response | None],
+    Coroutine[None, None, ResourceType | Response | None]
+    | ResourceType
+    | Response
+    | None,
 ]:
     """Make a function suitable for creation of a FHIR update API route."""
 
-    async def update(
-        request: Request,
-        response: Response,
-        id_: Id = Path(
-            None,
-            alias="id",
-            description=Resource.schema()["properties"]["id"]["title"],
-        ),
-        _format: str = FORMAT_QP,
-        _pretty: str = PRETTY_QP,
-        resource: ResourceType = Body(
-            None,
-            media_type="application/fhir+json",
-            alias=interaction.resource_type.get_resource_type(),
-        ),
-    ) -> ResourceType | Response | None:
-        if resource.id and id_ != resource.id:
-            raise FHIRBadRequestError(
-                code="invalid",
-                details_text="Logical Id in URL must match logical Id in resource",
+    if iscoroutinefunction(interaction.handler):
+
+        async def update_async(
+            request: Request,
+            response: Response,
+            id_: Id = Path(
+                None,
+                alias="id",
+                description=Resource.schema()["properties"]["id"]["title"],
+            ),
+            _format: str = FORMAT_QP,
+            _pretty: str = PRETTY_QP,
+            resource: ResourceType = Body(
+                None,
+                media_type="application/fhir+json",
+                alias=interaction.resource_type.get_resource_type(),
+            ),
+        ) -> ResourceType | Response | None:
+            """Function for update interaction."""
+            if resource.id and id_ != resource.id:
+                raise FHIRBadRequestError(
+                    code="invalid",
+                    details_text="Logical Id in URL must match logical Id in resource",
+                )
+
+            handler = cast(
+                UpdateInteractionAsyncHandler[ResourceType], interaction.handler
             )
+            result = await handler(InteractionContext(request, response), id_, resource)  # type: ignore
+            _, result_resource = _result_to_id_resource_tuple(result)
 
-        handler = cast(UpdateInteractionHandler[ResourceType], interaction.handler)
-        result = await handler(InteractionContext(request, response), id_, resource)  # type: ignore
-        _, result_resource = _result_to_id_resource_tuple(result)
-
-        return format_response(
-            resource=result_resource,
-            response=response,
-            format_parameters=FormatParameters.from_request(request),
-        )
+            return format_response(
+                resource=result_resource,
+                response=response,
+                format_parameters=FormatParameters.from_request(request),
+            )
 
-    update.__annotations__ |= {
-        "resource": interaction.resource_type,
-    }
+        update_async.__annotations__ |= {
+            "resource": interaction.resource_type,
+        }
+
+        return update_async
+    else:
+
+        def update(
+            request: Request,
+            response: Response,
+            id_: Id = Path(
+                None,
+                alias="id",
+                description=Resource.schema()["properties"]["id"]["title"],
+            ),
+            _format: str = FORMAT_QP,
+            _pretty: str = PRETTY_QP,
+            resource: ResourceType = Body(
+                None,
+                media_type="application/fhir+json",
+                alias=interaction.resource_type.get_resource_type(),
+            ),
+        ) -> ResourceType | Response | None:
+            """Function for update interaction."""
+            if resource.id and id_ != resource.id:
+                raise FHIRBadRequestError(
+                    code="invalid",
+                    details_text="Logical Id in URL must match logical Id in resource",
+                )
+
+            handler = cast(UpdateInteractionHandler[ResourceType], interaction.handler)
+            result = handler(InteractionContext(request, response), id_, resource)  # type: ignore
+            _, result_resource = _result_to_id_resource_tuple(result)
+
+            return format_response(
+                resource=result_resource,
+                response=response,
+                format_parameters=FormatParameters.from_request(request),
+            )
+
+        update.__annotations__ |= {
+            "resource": interaction.resource_type,
+        }
 
-    return update
+        return update
 
 
 def _result_to_id_resource_tuple(
-    result: Id | Resource,
-) -> tuple[Id | None, Resource | None]:
+    result: Id | ResourceType,
+) -> tuple[Id | None, ResourceType | None]:
     """
     Given an Id or a Resource, return an Id and a Resource.
 
     If a Resource is provided, both an Id and a Resource can be returned, however if an Id is
     provided, then only the Id can be returned.
     """
     if isinstance(result, Resource):
@@ -294,7 +442,38 @@
     """
     return not keyword.iskeyword(name) and name not in {
         "context",
         "format",
         "resource",
         "type",
     }
+
+
+def _set_search_type_function_signature(
+    search_type_function: Callable[
+        [Request, Response, str, str],
+        Coroutine[None, None, Bundle | Response] | Bundle | Response,
+    ],
+    search_parameters: tuple[Parameter, ...],
+    search_parameter_metadata: dict[str, dict[str, str]],
+) -> Callable[
+    [Request, Response, str, str],
+    Coroutine[None, None, Bundle | Response] | Bundle | Response,
+]:
+    """
+    Set the function signature of the search-type function so that it includes the search parameters
+    that the handler supports.
+    """
+    sig = signature(search_type_function)
+    parameters: tuple[Parameter, ...] = tuple(sig.parameters.values())[:-1]
+
+    sorted_search_parameters: list[Parameter] = sorted(
+        parameters + search_parameters,
+        key=lambda p: search_parameter_sort_key(
+            p.name, search_parameter_metadata, p.annotation
+        ),
+    )
+
+    sig = sig.replace(parameters=sorted_search_parameters)
+    setattr(search_type_function, "__signature__", sig)
+
+    return search_type_function
```

### Comparing `fhirstarter-0.13.9/fhirstarter/scripts/example.py` & `fhirstarter-1.0.0/fhirstarter/scripts/example.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from uuid import uuid4
 
 import uvicorn
 from fhir.resources.bundle import Bundle
 from fhir.resources.fhirtypes import Id
 from fhir.resources.humanname import HumanName
 from fhir.resources.patient import Patient
+from fhir.resources.practitioner import Practitioner
 from starlette.responses import RedirectResponse
 
 from fhirstarter import FHIRProvider, FHIRStarter, InteractionContext, Request, Response
 from fhirstarter.exceptions import FHIRResourceNotFoundError
 
 # Create the app with the provided config file
 app = FHIRStarter(
@@ -59,17 +60,18 @@
     return patient
 
 
 # Register the patient search-type FHIR interaction with the provider
 @provider.search_type(Patient)
 async def patient_search_type(
     context: InteractionContext,
+    birthdate: list[str] | None,
     general_practitioner: str | None,
     family: str | None,
-    nickname: list[str] | None,
+    nickname: str | None,
     _last_updated: str | None,
 ) -> Bundle:
     patients = []
     for patient in DATABASE.values():
         for name in patient.name:
             if cast(HumanName, name).family == family:
                 patients.append(patient)
@@ -93,14 +95,34 @@
 
     patient = deepcopy(resource)
     DATABASE[id_] = patient
 
     return Id(patient.id)
 
 
+# Optional: Provide a custom example for the automatic documentation by defining a subclass of the
+# FHIR Practitioner Pydantic model. If a custom model is not provided, examples from the FHIR
+# specification are used.
+class PractitionerCustom(Practitioner):
+    class Config:
+        schema_extra = {
+            "example": {
+                "resourceType": "Practitioner",
+                "id": "example",
+                "name": [{"family": "Careful", "given": ["Adam"], "prefix": ["Dr"]}],
+            }
+        }
+
+
+# Register the practitioner read FHIR interaction with the provider using the custom subclass
+@provider.read(PractitionerCustom)
+async def practitioner_read(context: InteractionContext, id_: Id) -> PractitionerCustom:
+    return PractitionerCustom(**PractitionerCustom.Config.schema_extra["example"])
+
+
 # Add the provider to the app. This will automatically generate the API routes for the interactions
 # provided by the providers (e.g. create, read, search-type, and update).
 app.add_providers(provider)
 
 
 # Customize the capability statement
 def amend_capability_statement(
```

### Comparing `fhirstarter-0.13.9/fhirstarter/search_parameters.py` & `fhirstarter-1.0.0/fhirstarter/search_parameters.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,77 +2,26 @@
 Functions for working with search parameters defined for search operations in the FHIR
 specification.
 """
 
 import inspect
 import re
 from collections.abc import Callable, Mapping
-from copy import deepcopy
 from dataclasses import dataclass
 from functools import cache
 from typing import Any
 
 from fastapi import Request, Response
 
-from .fhir_specification.utils import load_search_parameters
+from .fhir_specification.utils import (
+    load_extra_search_parameters,
+    load_search_parameters,
+)
 from .interactions import InteractionContext
 
-_EXTRA_SEARCH_PARAMETERS = {
-    "Resource": {
-        "_list": {
-            "type": "string",
-            "description": "All resources in nominated list (by id, Type/id, url or one of the "
-            "magic List types)",
-            "uri": "http://hl7.org/fhir/SearchParameter/Resource-list",
-            "include-in-capability-statement": True,
-        },
-        "_sort": {
-            "type": "string",
-            "description": "Order to sort results in (can repeat for inner sort "
-            "orders)\r\n\r\nAllowable Content: Name of a valid search parameter",
-            "include-in-capability-statement": False,
-        },
-        "_count": {
-            "type": "number",
-            "description": "Number of results per page\r\n\r\nAllowable Content: Whole number",
-            "include-in-capability-statement": False,
-        },
-        "_include": {
-            "type": "string",
-            "description": "Other resources to include in the search results that search matches "
-            "point to\r\n\r\nAllowable Content: SourceType:searchParam(:targetType)",
-            "include-in-capability-statement": False,
-        },
-        "_revinclude": {
-            "type": "string",
-            "description": "Other resources to include in the search results when they refer to "
-            "search matches\r\n\r\nAllowable Content: SourceType:searchParam(:targetType)",
-            "include-in-capability-statement": False,
-        },
-        "_summary": {
-            "type": "string",
-            "description": "Just return the summary elements (for resources where this is "
-            "defined)\r\n\r\nAllowable Content: true | false (false is default)",
-            "include-in-capability-statement": False,
-        },
-        "_contained": {
-            "type": "string",
-            "description": "Whether to return resources contained in other resources in the search "
-            "matches\r\n\r\nAllowable Content: true | false | both (false is default)",
-            "include-in-capability-statement": False,
-        },
-        "_containedType": {
-            "type": "string",
-            "description": "If returning contained resources, whether to return the contained or "
-            "container resources\r\n\r\nAllowable Content: container | contained",
-            "include-in-capability-statement": False,
-        },
-    }
-}
-
 
 class SearchParameters:
     def __init__(
         self,
         custom_search_parameters: Mapping[str, Mapping[str, Mapping[str, str]]]
         | None = None,
     ):
@@ -171,22 +120,22 @@
             "include-in-capability-statement", False
         ),
         var_name_to_qp_name(name),
     )
 
 
 @cache
-def _load_search_parameters_file() -> dict[str, dict[str, dict[str, str]]]:
+def _load_search_parameters_file() -> dict[str, dict[str, dict[str, str | bool]]]:
     """
     Load the search parameters JSON file.
 
     Organize the search parameter file by resource type and return a dict with the data. Initialize
     the search parameters dict with values that aren't present in the JSON file.
     """
-    search_parameters: dict = deepcopy(_EXTRA_SEARCH_PARAMETERS)
+    search_parameters = {"Resource": load_extra_search_parameters()}
 
     bundle = load_search_parameters()
 
     for entry in bundle["entry"]:
         resource = entry["resource"]
 
         for resource_type in resource["base"]:
@@ -207,13 +156,13 @@
     """
     Remove other descriptions in the case where the text contains descriptions for multiple resource
     types, and return only the description for the specified resource type.
     """
     if description.startswith("Multiple Resources:"):
         for description_for_resource_type in description.split("\n"):
             if description_for_resource_type.startswith(f"* [{resource_type}]"):
-                _, description = description_for_resource_type.split(": ")
+                _, description = description_for_resource_type.split(": ", maxsplit=1)
                 return description.removesuffix("\r")
         else:
             raise AssertionError("Resource type must exist in the description")
 
     return description
```

### Comparing `fhirstarter-0.13.9/fhirstarter/tests/config.py` & `fhirstarter-1.0.0/fhirstarter/tests/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,71 @@
 """FHIRStarter test configuration"""
 
 from copy import deepcopy
 from tempfile import NamedTemporaryFile
 from typing import cast
 
-from fhir.resources.bundle import Bundle
-from fhir.resources.fhirtypes import Id
-from fhir.resources.humanname import HumanName
-from fhir.resources.patient import Patient
-
 from ..exceptions import FHIRResourceNotFoundError
 from ..fhirstarter import FHIRStarter
 from ..interactions import InteractionContext
 from ..providers import FHIRProvider
+from ..resources import Bundle, Id
 from ..testclient import TestClient
+from .resources import HumanName, Patient
 from .utils import generate_fhir_resource_id
 
 # In-memory "database" used to simulate persistence of created FHIR resources
 DATABASE: dict[str, Patient] = {}
 
 _VALID_TOKEN = "valid"
 _INVALID_TOKEN = "invalid"
 
 
-async def patient_create(_: InteractionContext, resource: Patient) -> Id:
+async def patient_create_async(context: InteractionContext, resource: Patient) -> Id:
+    """Patient create FHIR interaction."""
+    return patient_create(context, resource)
+
+
+def patient_create(_: InteractionContext, resource: Patient) -> Id:
     """Patient create FHIR interaction."""
     patient = deepcopy(resource)
     patient.id = generate_fhir_resource_id()
     DATABASE[patient.id] = patient
 
     return Id(patient.id)
 
 
-async def patient_read(_: InteractionContext, id_: Id) -> Patient:
+async def patient_read_async(context: InteractionContext, id_: Id) -> Patient:
+    """Patient read FHIR interaction."""
+    return patient_read(context, id_)
+
+
+def patient_read(_: InteractionContext, id_: Id) -> Patient:
     """Patient read FHIR interaction."""
     patient = DATABASE.get(id_)
     if not patient:
         raise FHIRResourceNotFoundError
 
     return patient
 
 
-async def patient_search_type(
+async def patient_search_type_async(
+    context: InteractionContext,
+    family: str | None,
+    general_practitioner: str | None,
+    nickname: str | None,
+    _last_updated: str | None,
+) -> Bundle:
+    """Patient search-type FHIR interaction."""
+    return patient_search_type(
+        context, family, general_practitioner, nickname, _last_updated
+    )
+
+
+def patient_search_type(
     _: InteractionContext,
     family: str | None,
     general_practitioner: str | None,
     nickname: str | None,
     _last_updated: str | None,
 ) -> Bundle:
     """Patient search-type FHIR interaction."""
@@ -62,15 +82,22 @@
             "entry": [{"resource": patient.dict()} for patient in patients],
         }
     )
 
     return bundle
 
 
-async def patient_update(_: InteractionContext, id_: Id, resource: Patient) -> Id:
+async def patient_update_async(
+    context: InteractionContext, id_: Id, resource: Patient
+) -> Id:
+    """Patient update FHIR interaction."""
+    return patient_update(context, id_, resource)
+
+
+def patient_update(_: InteractionContext, id_: Id, resource: Patient) -> Id:
     """Patient update FHIR interaction."""
     if id_ not in DATABASE:
         raise FHIRResourceNotFoundError
 
     patient = deepcopy(resource)
     DATABASE[id_] = patient
 
@@ -95,25 +122,33 @@
     app.add_providers(provider)
 
     DATABASE.clear()
 
     return TestClient(app)
 
 
-def client() -> TestClient:
-    """Create an app that provides all FHIR interactions."""
+def create_test_client(
+    interactions: tuple[str, ...], async_endpoints: bool
+) -> TestClient:
+    """Given a list of interactions and an async flag, create an app and return a test client."""
     provider = FHIRProvider()
-    provider.create(Patient)(patient_create)
-    provider.read(Patient)(patient_read)
-    provider.search_type(Patient)(patient_search_type)
-    provider.update(Patient)(patient_update)
-
-    return app(provider)
 
-
-def client_create_and_read() -> TestClient:
-    """Create an app that only provides FHIR create and read interactions."""
-    provider = FHIRProvider()
-    provider.create(Patient)(patient_create)
-    provider.read(Patient)(patient_read)
+    for interaction in interactions:
+        match interaction, async_endpoints:
+            case "create", True:
+                provider.create(Patient)(patient_create_async)
+            case "create", False:
+                provider.create(Patient)(patient_create)
+            case "read", True:
+                provider.read(Patient)(patient_read_async)
+            case "read", False:
+                provider.read(Patient)(patient_read)
+            case "search-type", True:
+                provider.search_type(Patient)(patient_search_type_async)
+            case "search-type", False:
+                provider.search_type(Patient)(patient_search_type)
+            case "update", True:
+                provider.update(Patient)(patient_update_async)
+            case "update", False:
+                provider.update(Patient)(patient_update)
 
     return app(provider)
```

### Comparing `fhirstarter-0.13.9/fhirstarter/tests/test_capability_statement.py` & `fhirstarter-1.0.0/fhirstarter/tests/test_capability_statement.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Test the capability statement"""
-
 from collections.abc import Mapping, MutableMapping, Sequence
 from typing import Any, cast
 
 import pytest
-from fhir.resources.capabilitystatement import CapabilityStatement
 
 from .. import status
+from ..fhir_specification import FHIR_SEQUENCE, FHIR_VERSION
 from ..fhirstarter import FHIRStarter
+from ..resources import CapabilityStatement
 from ..testclient import TestClient
-from .config import client, client_create_and_read
 from .utils import assert_expected_response
 
 
 @pytest.mark.parametrize(
-    argnames="test_client,resource",
+    argnames="client,resource",
     argvalues=[
         (
-            client(),
+            ["create", "read", "search-type", "update"],
             [
                 {
                     "type": "Patient",
                     "interaction": [
                         {"code": "create"},
                         {"code": "read"},
                         {"code": "search-type"},
@@ -56,65 +55,65 @@
                             "documentation": "When the resource version last changed",
                         },
                     ],
                 }
             ],
         ),
         (
-            client_create_and_read(),
+            ["create", "read"],
             [
                 {
                     "type": "Patient",
                     "interaction": [{"code": "create"}, {"code": "read"}],
                 },
             ],
         ),
     ],
-    ids=["all", "create_and_read"],
+    ids=["all", "create and read"],
+    indirect=["client"],
 )
 def test_capability_statement(
-    test_client: TestClient, resource: Sequence[Mapping[str, Any]]
+    client: TestClient, resource: Sequence[Mapping[str, Any]]
 ) -> None:
     """
     Test the capability statement.
 
     Two scenarios are parameterized: a server with create, read, search, and update supported, and
     a server with only create and read supported.
     """
-    app = cast(FHIRStarter, test_client.app)
+    app = cast(FHIRStarter, client.app)
 
-    response = test_client.get("/metadata")
+    response = client.get("/metadata")
 
     assert_expected_response(
         response,
         status.HTTP_200_OK,
-        content={
-            "resourceType": "CapabilityStatement",
-            "status": "active",
-            "date": app._created.isoformat(),
-            "kind": "instance",
-            "fhirVersion": "4.0.1",
-            "format": ["json"],
-            "rest": [
-                {
-                    "mode": "server",
-                    "resource": resource,
-                }
-            ],
-        },
+        content=_fhir_sequence_adjust(
+            {
+                "resourceType": "CapabilityStatement",
+                "status": "active",
+                "date": app._created.isoformat(),
+                "kind": "instance",
+                "fhirVersion": FHIR_VERSION,
+                "acceptUnknown": "no",
+                "format": ["json"],
+                "rest": [
+                    {
+                        "mode": "server",
+                        "resource": resource,
+                    }
+                ],
+            }
+        ),
     )
 
 
-def test_capability_statement_pretty(
-    client_create_and_read_fixture: TestClient,
-) -> None:
+def test_capability_statement_pretty(client_create_and_read: TestClient) -> None:
     """Test the capability statement with a pretty response."""
-    test_client = client_create_and_read_fixture
-
-    response = test_client.get("/metadata?_pretty=true")
+    response = client_create_and_read.get("/metadata?_pretty=true")
 
     assert_expected_response(
         response,
         status.HTTP_200_OK,
         content=CapabilityStatement(**response.json()).json(
             indent=2, separators=(", ", ": ")
         ),
@@ -123,65 +122,76 @@
 
 @pytest.mark.parametrize(
     argnames="pretty",
     argvalues=["false", "true"],
     ids=["minified", "pretty"],
 )
 def test_capability_statement_xml(
-    client_create_and_read_fixture: TestClient, pretty: str
+    client_create_and_read: TestClient, pretty: str
 ) -> None:
     """Test the capability statement with an XML response."""
-    test_client = client_create_and_read_fixture
-
-    response = test_client.get(f"/metadata?_format=xml&_pretty={pretty}")
+    response = client_create_and_read.get(f"/metadata?_format=xml&_pretty={pretty}")
 
     assert_expected_response(
         response,
         status.HTTP_200_OK,
         content_type="application/fhir+xml",
         content=CapabilityStatement.parse_raw(
             response.content, content_type="text/xml"
         ).xml(pretty_print=(pretty == "true")),
     )
 
 
-def test_set_capability_statement_modifier(
-    client_create_and_read_fixture: TestClient,
-) -> None:
+def test_set_capability_statement_modifier(client_create_and_read: TestClient) -> None:
     """Test the set_capability_statement_modifier method."""
-    test_client = client_create_and_read_fixture
-    app = cast(FHIRStarter, test_client.app)
+    app = cast(FHIRStarter, client_create_and_read.app)
 
     def modify_capability_statement(
         capability_statement: MutableMapping[str, Any], *_: Any
     ) -> MutableMapping[str, Any]:
         capability_statement["publisher"] = "Publisher"
         return capability_statement
 
     app.set_capability_statement_modifier(modify_capability_statement)
 
-    response = test_client.get("/metadata")
+    response = client_create_and_read.get("/metadata")
 
     assert_expected_response(
         response,
         status.HTTP_200_OK,
-        content={
-            "resourceType": "CapabilityStatement",
-            "status": "active",
-            "date": app._created.isoformat(),
-            "publisher": "Publisher",
-            "kind": "instance",
-            "fhirVersion": "4.0.1",
-            "format": ["json"],
-            "rest": [
-                {
-                    "mode": "server",
-                    "resource": [
-                        {
-                            "type": "Patient",
-                            "interaction": [{"code": "create"}, {"code": "read"}],
-                        }
-                    ],
-                }
-            ],
-        },
+        content=_fhir_sequence_adjust(
+            {
+                "resourceType": "CapabilityStatement",
+                "status": "active",
+                "date": app._created.isoformat(),
+                "publisher": "Publisher",
+                "kind": "instance",
+                "fhirVersion": FHIR_VERSION,
+                "acceptUnknown": "no",
+                "format": ["json"],
+                "rest": [
+                    {
+                        "mode": "server",
+                        "resource": [
+                            {
+                                "type": "Patient",
+                                "interaction": [{"code": "create"}, {"code": "read"}],
+                            }
+                        ],
+                    }
+                ],
+            }
+        ),
     )
+
+
+def _fhir_sequence_adjust(
+    capability_statement: MutableMapping[str, Any]
+) -> MutableMapping[str, Any]:
+    """
+    Adjust a capability statement for the purposes of comparison.
+    Example: For R4, R4B, and R5, the "acceptUnknown" value is no longer present.
+    """
+    if FHIR_SEQUENCE != "STU3":
+        del capability_statement["acceptUnknown"]
+
+    return capability_statement
```

### Comparing `fhirstarter-0.13.9/fhirstarter/tests/test_dependencies.py` & `fhirstarter-1.0.0/fhirstarter/tests/test_dependencies.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Test FHIRStarter dependency injection"""
 
 import pytest
+from _pytest.fixtures import FixtureRequest
 from fastapi import Depends
 from fastapi.security import HTTPAuthorizationCredentials, HTTPBearer
-from fhir.resources.patient import Patient
 
 from ..exceptions import FHIRUnauthorizedError
 from ..fhirstarter import FHIRProvider, status
-from .config import app, patient_create
+from .config import app, patient_create, patient_create_async
+from .resources import Patient
 from .utils import assert_expected_response, resource
 
 _VALID_TOKEN = "valid"
 _INVALID_TOKEN = "invalid"
 
 
 def validate_token(
@@ -20,35 +21,50 @@
     """
     Ensure that the authorization credentials are bearer credentials with a valid access token.
     """
     if authorization.scheme != "Bearer" or authorization.credentials != _VALID_TOKEN:
         raise FHIRUnauthorizedError(details_text="Authentication failed")
 
 
-def provider_with_dependency() -> FHIRProvider:
+@pytest.fixture
+def provider_with_dependency(async_endpoints: bool) -> FHIRProvider:
     """Create a provider with a provider-level dependency."""
     provider = FHIRProvider(dependencies=[Depends(validate_token)])
-    provider.create(Patient)(patient_create)
+    provider.create(Patient)(
+        patient_create_async if async_endpoints else patient_create
+    )
 
     return provider
 
 
-def provider_with_interaction_dependency() -> FHIRProvider:
+@pytest.fixture
+def provider_with_interaction_dependency(async_endpoints: bool) -> FHIRProvider:
     """Create a provider with an interaction-level dependency."""
     provider = FHIRProvider()
-    provider.create(Patient, dependencies=[Depends(validate_token)])(patient_create)
+    provider.create(Patient, dependencies=[Depends(validate_token)])(
+        patient_create_async if async_endpoints else patient_create
+    )
 
     return provider
 
 
-@pytest.mark.parametrize(
-    argnames="provider",
-    argvalues=[provider_with_dependency(), provider_with_interaction_dependency()],
-    ids=["provider", "interaction"],
-)
+@pytest.fixture(params=[True, False], ids=["provider", "interaction"])
+def provider(
+    request: FixtureRequest,
+    provider_with_dependency: FHIRProvider,
+    provider_with_interaction_dependency: FHIRProvider,
+) -> FHIRProvider:
+    """Parametrized fixture that returns a provider with a dependency added at different layers."""
+    return (
+        provider_with_dependency
+        if request.param
+        else provider_with_interaction_dependency
+    )
+
+
 def test_dependency(provider: FHIRProvider) -> None:
     """Test that injected token validation dependency works on the given provider."""
     client = app(provider)
 
     create_response = client.post(
         "/Patient",
         json=resource(),
```

### Comparing `fhirstarter-0.13.9/fhirstarter/tests/test_interactions.py` & `fhirstarter-1.0.0/fhirstarter/tests/test_interactions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,108 +1,121 @@
 """Test FHIR interactions"""
 
-from collections.abc import Callable
+from collections.abc import Callable, Coroutine
 from functools import partial
+from inspect import iscoroutinefunction
 from typing import cast
 
 import pytest
-from fhir.resources.bundle import Bundle
-from fhir.resources.humanname import HumanName
-from fhir.resources.patient import Patient
 from requests.models import Response
 
 from .. import status
 from ..interactions import InteractionContext
 from ..providers import FHIRProvider
+from ..resources import Bundle
 from ..testclient import TestClient
 from ..utils import make_operation_outcome
-from .config import DATABASE, app, patient_create
+from .config import (
+    DATABASE,
+    app,
+    create_test_client,
+    patient_create,
+    patient_create_async,
+)
+from .resources import HumanName, Patient
 from .utils import (
     assert_expected_response,
     generate_fhir_resource_id,
     id_from_create_response,
     json_dumps_pretty,
     resource,
 )
 
 
-def test_create(create_response_fixture: Response) -> None:
+@pytest.fixture(scope="module")
+def client(async_endpoints: bool) -> TestClient:
+    """Return a module-scoped test client with all interactions enabled."""
+    return create_test_client(
+        interactions=("create", "read", "search-type", "update"),
+        async_endpoints=async_endpoints,
+    )
+
+
+@pytest.fixture(scope="module")
+def create_response(client: TestClient) -> Response:
+    """Return the response from a Patient create interaction."""
+    return client.post("/Patient", json=resource())
+
+
+@pytest.fixture(scope="module")
+def patient_id(create_response: Response) -> str:
+    """Return the patient ID from a Patient create interaction."""
+    return id_from_create_response(create_response)
+
+
+def test_create(create_response: Response) -> None:
     """Test FHIR create interaction."""
-    assert_expected_response(create_response_fixture, status.HTTP_201_CREATED)
+    assert_expected_response(create_response, status.HTTP_201_CREATED)
 
 
-def test_read(client_fixture: TestClient, create_response_fixture: Response) -> None:
+def test_read(client: TestClient, patient_id: str) -> None:
     """Test FHIR read interaction."""
-    client = client_fixture
-
-    id_ = id_from_create_response(create_response_fixture)
-    read_response = client.get(f"/Patient/{id_}")
+    read_response = client.get(f"/Patient/{patient_id}")
 
-    assert_expected_response(read_response, status.HTTP_200_OK, content=resource(id_))
+    assert_expected_response(
+        read_response, status.HTTP_200_OK, content=resource(patient_id)
+    )
 
 
-def test_read_pretty(
-    client_fixture: TestClient, create_response_fixture: Response
-) -> None:
+def test_read_pretty(client: TestClient, patient_id: str) -> None:
     """Test FHIR read interaction with a pretty response."""
-    client = client_fixture
-
-    id_ = id_from_create_response(create_response_fixture)
-    read_response = client.get(f"/Patient/{id_}?_pretty=true")
+    read_response = client.get(f"/Patient/{patient_id}?_pretty=true")
 
     assert_expected_response(
-        read_response, status.HTTP_200_OK, content=json_dumps_pretty(resource(id_))
+        read_response,
+        status.HTTP_200_OK,
+        content=json_dumps_pretty(resource(patient_id)),
     )
 
 
 @pytest.mark.parametrize(
     argnames="pretty",
     argvalues=["false", "true"],
     ids=["minified", "pretty"],
 )
-def test_read_xml(
-    client_fixture: TestClient, create_response_fixture: Response, pretty: str
-) -> None:
+def test_read_xml(client: TestClient, patient_id: str, pretty: str) -> None:
     """Test FHIR read interaction with an XML response."""
-    client = client_fixture
-
-    id_ = id_from_create_response(create_response_fixture)
-
-    read_response = client.get(f"/Patient/{id_}?_format=xml&_pretty={pretty}")
+    read_response = client.get(f"/Patient/{patient_id}?_format=xml&_pretty={pretty}")
 
     assert_expected_response(
         read_response,
         status.HTTP_200_OK,
         content_type="application/fhir+xml",
-        content=Patient(**(resource(id_))).xml(pretty_print=(pretty == "true")),
+        content=Patient(**(resource(patient_id))).xml(pretty_print=(pretty == "true")),
     )
 
 
-def test_read_not_found(client_fixture: TestClient) -> None:
+def test_read_not_found(client: TestClient) -> None:
     """Test FHIR read interaction that produces a 404 not found error."""
-    client = client_fixture
-
     id_ = generate_fhir_resource_id()
     read_response = client.get(f"/Patient/{id_}")
 
     assert_expected_response(
         read_response,
         status.HTTP_404_NOT_FOUND,
         content=make_operation_outcome(
             severity="error",
             code="not-found",
             details_text=f"Unknown Patient resource '{id_}'",
         ).dict(),
     )
 
 
-def test_read_not_found_pretty(client_fixture: TestClient) -> None:
+def test_read_not_found_pretty(client: TestClient) -> None:
     """Test FHIR read interaction that produces a 404 not found error with a pretty response."""
-    client = client_fixture
-
     id_ = generate_fhir_resource_id()
     read_response = client.get(f"/Patient/{id_}?_pretty=true")
 
     assert_expected_response(
         read_response,
         status.HTTP_404_NOT_FOUND,
         content=json_dumps_pretty(
@@ -116,18 +129,16 @@
 
 
 @pytest.mark.parametrize(
     argnames="pretty",
     argvalues=["false", "true"],
     ids=["minified", "pretty"],
 )
-def test_read_not_found_xml(client_fixture: TestClient, pretty: str) -> None:
+def test_read_not_found_xml(client: TestClient, pretty: str) -> None:
     """Test FHIR read interaction that produces a 404 not found error with an XML response."""
-    client = client_fixture
-
     id_ = generate_fhir_resource_id()
     read_response = client.get(f"/Patient/{id_}?_format=xml&_pretty={pretty}")
 
     assert_expected_response(
         read_response,
         status.HTTP_404_NOT_FOUND,
         content_type="application/fhir+xml",
@@ -150,37 +161,70 @@
             lambda client: partial(client.post, "/Patient/_search"),
             {"data": {"family": "Baggins"}},
         ),
     ],
     ids=["get", "post"],
 )
 def test_search_type(
-    client_fixture: TestClient,
-    create_response_fixture: Response,
+    client: TestClient,
+    patient_id: str,
     search_type_func: Callable[[TestClient], Callable[..., Response]],
     search_type_func_kwargs: dict[str, str],
 ) -> None:
     """Test the FHIR search interaction."""
-    client = client_fixture
-
-    id_ = id_from_create_response(create_response_fixture)
     search_type_response = search_type_func(client)(**search_type_func_kwargs)
 
     assert_expected_response(
         search_type_response,
         status.HTTP_200_OK,
         content={
             "resourceType": "Bundle",
             "type": "searchset",
             "total": 1,
-            "entry": [{"resource": resource(id_)}],
+            "entry": [{"resource": resource(patient_id)}],
         },
     )
 
 
+def _search_type_handler_parameter_multiple_values_async() -> (
+    Callable[..., Coroutine[None, None, Bundle]]
+):
+    """Return an async Patient search-type handler that can test repeated query parameters."""
+
+    async def patient_search_type(
+        context: InteractionContext, given: list[str] | None
+    ) -> Bundle:
+        return _search_type_handler_parameter_multiple_values()(context, given)
+
+    return patient_search_type
+
+
+def _search_type_handler_parameter_multiple_values() -> Callable[..., Bundle]:
+    """Return a Patient search-type handler that can test repeated query parameters."""
+
+    def patient_search_type(_: InteractionContext, given: list[str] | None) -> Bundle:
+        patients = []
+        for patient in DATABASE.values():
+            for name in patient.name:
+                if set(given).issubset(cast(HumanName, name).given):
+                    patients.append(patient)
+
+        bundle = Bundle(
+            **{
+                "type": "searchset",
+                "total": len(patients),
+                "entry": [{"resource": patient.dict()} for patient in patients],
+            }
+        )
+
+        return bundle
+
+    return patient_search_type
+
+
 @pytest.mark.parametrize(
     argnames="search_type_func,search_type_func_kwargs,search_type_func_kwargs_zero_results",
     argvalues=[
         (
             lambda client: partial(client.get, "/Patient"),
             {"params": {"given": ["Samwise", "Sam"]}},
             {"params": {"given": ["Samwise", "Frodo"]}},
@@ -189,51 +233,45 @@
             lambda client: partial(client.post, "/Patient/_search"),
             {"data": {"given": ["Samwise", "Sam"]}},
             {"data": {"given": ["Samwise", "Frodo"]}},
         ),
     ],
     ids=["get", "post"],
 )
+@pytest.mark.parametrize(
+    argnames="handler",
+    argvalues=[
+        _search_type_handler_parameter_multiple_values_async(),
+        _search_type_handler_parameter_multiple_values(),
+    ],
+    ids=["async", "nonasync"],
+)
 def test_search_type_parameter_multiple_values(
+    handler: Callable[..., Coroutine[None, None, Bundle]] | Callable[..., Bundle],
     search_type_func: Callable[[TestClient], Callable[..., Response]],
     search_type_func_kwargs: dict[str, str],
     search_type_func_kwargs_zero_results: dict[str, str],
 ) -> None:
     """Test the FHIR search interaction with a parameter that has multiple values."""
+    provider = FHIRProvider()
 
-    async def patient_search_type(
-        _: InteractionContext, given: list[str] | None
-    ) -> Bundle:
-        patients = []
-        for patient in DATABASE.values():
-            for name in patient.name:
-                if set(given).issubset(cast(HumanName, name).given):
-                    patients.append(patient)
-
-        bundle = Bundle(
-            **{
-                "type": "searchset",
-                "total": len(patients),
-                "entry": [{"resource": patient.dict()} for patient in patients],
-            }
-        )
-
-        return bundle
+    if iscoroutinefunction(handler):
+        provider.create(Patient)(patient_create_async)
+    else:
+        provider.create(Patient)(patient_create)
 
-    provider = FHIRProvider()
-    provider.create(Patient)(patient_create)
-    provider.search_type(Patient)(patient_search_type)
+    provider.search_type(Patient)(handler)
 
     client = app(provider)
 
     create_response = client.post(
         "/Patient",
         json={
             "resourceType": "Patient",
-            "name": [{"family": "Gangee", "given": ["Samwise", "Sam"]}],
+            "name": [{"family": "Gamgee", "given": ["Samwise", "Sam"]}],
         },
     )
     id_ = id_from_create_response(create_response)
 
     search_type_response = search_type_func(client)(**search_type_func_kwargs)
     assert_expected_response(
         search_type_response,
@@ -243,15 +281,15 @@
             "type": "searchset",
             "total": 1,
             "entry": [
                 {
                     "resource": {
                         "resourceType": "Patient",
                         "id": id_,
-                        "name": [{"family": "Gangee", "given": ["Samwise", "Sam"]}],
+                        "name": [{"family": "Gamgee", "given": ["Samwise", "Sam"]}],
                     }
                 }
             ],
         },
     )
 
     search_type_response = search_type_func(client)(
@@ -264,71 +302,61 @@
             "resourceType": "Bundle",
             "type": "searchset",
             "total": 0,
         },
     )
 
 
-def test_update(client_fixture: TestClient, create_response_fixture: Response) -> None:
+def test_update(client: TestClient, patient_id: str) -> None:
     """Test FHIR update interaction."""
-    client = client_fixture
-
-    id_ = id_from_create_response(create_response_fixture)
-    read_response = client.get(f"/Patient/{id_}")
+    read_response = client.get(f"/Patient/{patient_id}")
     content = read_response.json()
     content["name"][0]["given"][0] = "Frodo"
-    put_response = client.put(f"/Patient/{id_}", json=content)
+    put_response = client.put(f"/Patient/{patient_id}", json=content)
 
     assert_expected_response(put_response, status.HTTP_200_OK)
 
-    read_response = client.get(f"/Patient/{id_}")
+    read_response = client.get(f"/Patient/{patient_id}")
 
     assert_expected_response(
         read_response,
         status.HTTP_200_OK,
         content={
             "resourceType": "Patient",
-            "id": id_,
+            "id": patient_id,
             "name": [{"family": "Baggins", "given": ["Frodo"]}],
         },
     )
 
 
-def test_update_not_found(client_fixture: TestClient) -> None:
+def test_update_not_found(client: TestClient) -> None:
     """Test FHIR update interaction that produces a 404 not found error."""
-    client = client_fixture
-
     id_ = generate_fhir_resource_id()
     put_response = client.put(f"/Patient/{id_}", json=resource())
 
     assert_expected_response(
         put_response,
         status.HTTP_404_NOT_FOUND,
         content=make_operation_outcome(
             severity="error",
             code="not-found",
             details_text=f"Unknown Patient resource '{id_}'",
         ).dict(),
     )
 
 
-def test_update_id_mismatch(
-    client_fixture: TestClient, create_response_fixture: Response
-) -> None:
+def test_update_id_mismatch(client: TestClient, patient_id: str) -> None:
     """
     Test FHIR update interaction where the logical Id in the URL does not match the logical ID in
     the resource.
     """
-    client = client_fixture
-
-    id_ = id_from_create_response(create_response_fixture)
-    read_response = client.get(f"/Patient/{id_}")
+    read_response = client.get(f"/Patient/{patient_id}")
     content = read_response.json()
     content["id"] = generate_fhir_resource_id()
-    put_response = client.put(f"/Patient/{id_}", json=content)
+    put_response = client.put(f"/Patient/{patient_id}", json=content)
 
     assert_expected_response(
         put_response,
         status.HTTP_400_BAD_REQUEST,
         content={
             "resourceType": "OperationOutcome",
             "issue": [
```

### Comparing `fhirstarter-0.13.9/fhirstarter/tests/test_utils.py` & `fhirstarter-1.0.0/fhirstarter/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-0.13.9/fhirstarter/tests/utils.py` & `fhirstarter-1.0.0/fhirstarter/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import json
 from collections.abc import Mapping
 from typing import Any
 from urllib.parse import urlparse
 from uuid import uuid4
 
-from fhir.resources.fhirtypes import Id
 from funcy import omit
 from requests.models import Response
 
 from .. import Request
+from ..resources import Id
 
 _RESOURCE = {
     "resourceType": "Patient",
     "id": "",
     "name": [{"family": "Baggins", "given": ["Bilbo"]}],
 }
```

### Comparing `fhirstarter-0.13.9/fhirstarter/utils.py` & `fhirstarter-1.0.0/fhirstarter/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 import logging
 from collections.abc import Callable
 from dataclasses import dataclass
 from typing import Any, ClassVar, Literal
 
 from fastapi import Request
 from fastapi.responses import JSONResponse, Response
-from fhir.resources.bundle import Bundle
-from fhir.resources.operationoutcome import OperationOutcome
-from fhir.resources.resource import Resource
 
 from . import status
 from .fhir_specification.utils import is_resource_type
 from .interactions import ResourceType, SearchTypeInteraction, TypeInteraction
+from .resources import Bundle, OperationOutcome, Resource
 
 
 @dataclass
 class InteractionInfo:
     resource_type: str | None
     interaction_type: Literal[
         "create", "read", "update", "search-type", "capabilities"
@@ -229,15 +227,20 @@
         ), "Response object must be provided for a null resource"
         response.headers["Content-Type"] = format_parameters.format
         return resource
 
     if format_parameters.format == "application/fhir+json":
         if format_parameters.pretty:
             return Response(
-                content=resource.json(indent=2, separators=(", ", ": ")),
+                content=resource.json(
+                    ensure_ascii=False,
+                    allow_nan=False,
+                    indent=2,
+                    separators=(", ", ": "),
+                ),
                 status_code=status_code or status.HTTP_200_OK,
                 media_type=format_parameters.format,
             )
         else:
             if status_code:
                 return JSONResponse(
                     content=resource.dict(),
@@ -329,15 +332,15 @@
             interaction,
             _ok,
             _bad_request,
             _unauthorized,
             _forbidden,
             _internal_server_error,
         ),
-        "operation_id": f"fhirstarter|type|search|{'post' if post else 'get'}|{resource_type_str}",
+        "operation_id": f"fhirstarter|type|search-type|{'post' if post else 'get'}|{resource_type_str}",
         "response_model_exclude_none": True,
         **interaction.route_options,
     }
 
 
 def update_route_args(interaction: TypeInteraction[ResourceType]) -> dict[str, Any]:
     """Provide arguments for creation of a FHIR update API route."""
```

### Comparing `fhirstarter-0.13.9/pyproject.toml` & `fhirstarter-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fhirstarter"
-version = "0.13.9"
+version = "1.0.0"
 description = "An ASGI FHIR API framework built on top of FastAPI and FHIR Resources"
 authors = ["Christopher Sande <christopher.sande@canvasmedical.com>"]
 maintainers = ["Canvas Medical Engineering <engineering@canvasmedical.com>"]
 readme = "README.md"
 homepage = "https://github.com/canvas-medical/fhirstarter"
 repository = "https://github.com/canvas-medical/fhirstarter"
 keywords = ["fhir", "api", "resources", "framework", "fastapi", "healthcare", "hl7"]
@@ -29,15 +29,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.94.1"
-"fhir.resources" = "~6.4.0"
+"fhir.resources" = ">=6.4.0"
 lxml = "^4.9.2"
 python-multipart = "^0.0.6"
 uvloop = "^0.17.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 funcy = ">=1.18,<3.0"
```

### Comparing `fhirstarter-0.13.9/PKG-INFO` & `fhirstarter-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhirstarter
-Version: 0.13.9
+Version: 1.0.0
 Summary: An ASGI FHIR API framework built on top of FastAPI and FHIR Resources
 Home-page: https://github.com/canvas-medical/fhirstarter
 Keywords: fhir,api,resources,framework,fastapi,healthcare,hl7
 Author: Christopher Sande
 Author-email: christopher.sande@canvasmedical.com
 Maintainer: Canvas Medical Engineering
 Maintainer-email: engineering@canvasmedical.com
@@ -26,15 +26,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: fastapi (>=0.94.1,<0.95.0)
-Requires-Dist: fhir.resources (>=6.4.0,<6.5.0)
+Requires-Dist: fhir.resources (>=6.4.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Project-URL: Repository, https://github.com/canvas-medical/fhirstarter
 Description-Content-Type: text/markdown
 
 # fhirstarter
@@ -53,18 +53,22 @@
     <img src="https://img.shields.io/pypi/l/fhirstarter">
   </a>
   <a href="https://github.com/psf/black">
     <img src="https://img.shields.io/badge/code%20style-black-000000">
   </a>
 </p>
 
-An ASGI FHIR API framework built on top of [FastAPI](https://fastapi.tiangolo.com) and
+An ASGI [FHIR](https://hl7.org/fhir/) API framework built on top of [FastAPI](https://fastapi.tiangolo.com) and
 [FHIR Resources](https://pypi.org/project/fhir.resources/).
 
-The only version of FHIR that is currently supported is 4.0.1.
+Supports FHIR sequences:
+* [STU (v3.0.2)](https://hl7.org/fhir/STU3/)
+* [R4 (v4.0.1)](https://hl7.org/fhir/R4/)
+* [R4B (v4.3.0)](https://hl7.org/fhir/R4B/)
+* [R5 (v5.0.0)](https://hl7.org/fhir/R5/)
 
 ## Installation
 
 ```bash
 pip install fhirstarter
 ```
 
@@ -76,39 +80,74 @@
   API route
 * An exception-handling framework that produces FHIR-friendly responses (i.e. OperationOutcomes)
 * Automatically-generated, integrated documentation generated from the FHIR specification
 * Custom search parameters for search endpoints
 
 ### Disclaimer
 
-FHIRStarter was built based on the business needs of Canvas Medical. At any point in time, it may
-not be broadly applicable to the industry at large. Canvas Medical open-sourced the project so that
-it can be used by healthcare software developers whose needs it might also meet. Ongoing support and
-development will be based on the business needs of Canvas Medical.
+FHIRStarter was built based on the business needs of
+[Canvas Medical](https://www.canvasmedical.com). At any point in time, it may not be broadly
+applicable to the industry at large. Canvas Medical open-sourced the project so that it can be used
+by healthcare software developers whose needs it might also meet. Ongoing support and development
+will be based on the business needs of Canvas Medical.
 
 ## Background
 
-FHIRStarter uses a provider-decorator pattern. Developers can write functions that implement FHIR
-interactions -- such as create, read, search-type, and update -- and plug them into the framework.
-FHIRStarter then automatically creates FHIR-compatible API routes from these developer-provided
-functions. FHIR interactions that are supplied must use the resource classes defined by the
-[FHIR Resources](https://pypi.org/project/fhir.resources/) Python package, which is a collection of
-Pydantic models for FHIR resources.
+FHIRStarter uses a provider-decorator pattern. Developers can write functions, or handlers, that
+implement FHIR interactions -- such as create, read, search-type, and update -- and plug them into
+the framework. FHIRStarter then automatically creates FHIR-compatible API routes from these
+developer-provided functions. FHIR interactions that are supplied must use the resource classes
+defined by the [FHIR Resources](https://pypi.org/project/fhir.resources/) Python package, which is a
+collection of Pydantic models for FHIR resources.
 
 In order to stand up a FHIR server, all that is required is to create a FHIRStarter and a
 FHIRProvider instance, register a FHIR interaction with the provider, add the provider to the
 FHIRStarter instance, and pass the FHIRStarter instance to an ASGI server.
 
 ## Usage
 
 ### Currently-supported functionality
 
-FHIRStarter supports create, read, search-type, and update endpoints across all FHIR R4 resource
+FHIRStarter supports create, read, search-type, and update endpoints across all FHIR resource
 types, and will automatically generate the `/metadata` capabilities statement endpoint.
 
+Handlers can be written as coroutines with `async/await` syntax, or as plain functions. FastAPI
+supports both, as does FHIRStarter.
+
+### Configuration for specific FHIR sequences
+
+FHIRStarter will work out of the box as an R5 server. If a different sequence is desired, it must be
+specified with an environment variable:
+
+```shell
+FHIR_SEQUENCE="R4B"
+```
+
+The latest version of the [FHIR Resources](https://pypi.org/project/fhir.resources/) package only
+supports FHIR STU3, R4B, and R5. FHIR R4 is supported by an earlier version. Because of this, if a
+developer desires to use FHIR R4, then the developer must pin version **6.4.0** of fhir.resources in
+their project. FHIRStarter will check the version of fhir.resources against the specified FHIR
+version in the environment variable to ensure that they are compatible.
+
+Model imports are also affected by which version of fhir.resources is installed. For STU3 and R4B,
+model imports will look like this:
+
+```python
+from fhir.resources.STU3.patient import Patient
+```
+```python
+from fhir.resources.R4B.patient import Patient
+```
+
+For R4 and R5, model imports will look like this:
+
+```python
+from fhir.resources.patient import Patient
+```
+
 ### Example
 
 A detailed example is available here: [example.py](https://github.com/canvas-medical/fhirstarter/blob/main/fhirstarter/scripts/example.py).
 
 ```python
 import uvicorn
 from fhir.resources.fhirtypes import Id
@@ -191,16 +230,7 @@
 Dependencies specified at the application level will be injected into all routes in the application.
 
 Dependencies specified at the provider level will be injected into all routes that are added to
 the application from that specific provider.
 
 Dependencies specified at the handler level only apply to that specific FHIR interaction.
 
-## Forward compatibility
-
-At some point in the future, it will be necessary to support FHIR R5. How this might be supported on
-a server that continues to support R4 has not yet been determined (e.g. a header that specifies the
-version, adding the FHIR version to the URL path, etc.). It may be necessary to support alteration
-of how the URL path is specified through the provider construct. Currently, the FHIR version is not
-part of the URL path, so the default behavior is that an API route defined as `/Patient` will be an
-R4 endpoint.
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fhirstarter Version: 0.13.9 Summary: An ASGI FHIR
+Metadata-Version: 2.1 Name: fhirstarter Version: 1.0.0 Summary: An ASGI FHIR
 API framework built on top of FastAPI and FHIR Resources Home-page: https://
 github.com/canvas-medical/fhirstarter Keywords:
 fhir,api,resources,framework,fastapi,healthcare,hl7 Author: Christopher Sande
 Author-email: christopher.sande@canvasmedical.com Maintainer: Canvas Medical
 Engineering Maintainer-email: engineering@canvasmedical.com Requires-Python:
 >=3.11,<4.0 Classifier: Development Status :: 4 - Beta Classifier: Environment
 :: Web Environment Classifier: Framework :: AsyncIO Classifier: Framework ::
@@ -14,64 +14,81 @@
 Programming Language :: Python :: 3.11 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/
 HTTP :: HTTP Servers Classifier: Topic :: Software Development Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Application Frameworks Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Typing :: Typed
 Requires-Dist: fastapi (>=0.94.1,<0.95.0) Requires-Dist: fhir.resources
-(>=6.4.0,<6.5.0) Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist: python-
-multipart (>=0.0.6,<0.0.7) Requires-Dist: uvloop (>=0.17.0,<0.18.0) Project-
-URL: Repository, https://github.com/canvas-medical/fhirstarter Description-
-Content-Type: text/markdown # fhirstarter
+(>=6.4.0) Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist: python-multipart
+(>=0.0.6,<0.0.7) Requires-Dist: uvloop (>=0.17.0,<0.18.0) Project-URL:
+Repository, https://github.com/canvas-medical/fhirstarter Description-Content-
+Type: text/markdown # fhirstarter
 [https://github.com/canvas-medical/fhirstarter/actions/workflows/test.yml/
 badge.svg] [https://img.shields.io/pypi/v/fhirstarter] [https://img.shields.io/
 pypi/pyversions/fhirstarter] [https://img.shields.io/pypi/l/fhirstarter]
 [https://img.shields.io/badge/code%20style-black-000000]
-An ASGI FHIR API framework built on top of [FastAPI](https://
-fastapi.tiangolo.com) and [FHIR Resources](https://pypi.org/project/
-fhir.resources/). The only version of FHIR that is currently supported is
-4.0.1. ## Installation ```bash pip install fhirstarter ``` ## Features *
-Automatic, standardized API route creation * Automatic validation of inputs and
-outputs through the use of FHIR Resources Pydantic models * Automatically-
-generated capability statement that can be customized, and a capability
-statement API route * An exception-handling framework that produces FHIR-
-friendly responses (i.e. OperationOutcomes) * Automatically-generated,
-integrated documentation generated from the FHIR specification * Custom search
-parameters for search endpoints ### Disclaimer FHIRStarter was built based on
-the business needs of Canvas Medical. At any point in time, it may not be
-broadly applicable to the industry at large. Canvas Medical open-sourced the
-project so that it can be used by healthcare software developers whose needs it
-might also meet. Ongoing support and development will be based on the business
-needs of Canvas Medical. ## Background FHIRStarter uses a provider-decorator
-pattern. Developers can write functions that implement FHIR interactions -
-- such as create, read, search-type, and update -- and plug them into the
-framework. FHIRStarter then automatically creates FHIR-compatible API routes
-from these developer-provided functions. FHIR interactions that are supplied
-must use the resource classes defined by the [FHIR Resources](https://pypi.org/
-project/fhir.resources/) Python package, which is a collection of Pydantic
-models for FHIR resources. In order to stand up a FHIR server, all that is
-required is to create a FHIRStarter and a FHIRProvider instance, register a
-FHIR interaction with the provider, add the provider to the FHIRStarter
-instance, and pass the FHIRStarter instance to an ASGI server. ## Usage ###
-Currently-supported functionality FHIRStarter supports create, read, search-
-type, and update endpoints across all FHIR R4 resource types, and will
-automatically generate the `/metadata` capabilities statement endpoint. ###
-Example A detailed example is available here: [example.py](https://github.com/
-canvas-medical/fhirstarter/blob/main/fhirstarter/scripts/example.py). ```python
-import uvicorn from fhir.resources.fhirtypes import Id from
-fhir.resources.patient import Patient from fhirstarter import FHIRProvider,
-FHIRStarter, InteractionContext from fhirstarter.exceptions import
-FHIRResourceNotFoundError # Create the app app = FHIRStarter() # Create a
-provider provider = FHIRProvider() # Register the patient read FHIR interaction
-with the provider @provider.read(Patient) async def patient_read(context:
-InteractionContext, id_: Id) -> Patient: # Get the patient from the database
-patient = ... if not patient: raise FHIRResourceNotFoundError return Patient
-( **{ # Map patient from database to FHIR Patient structure } ) # Add the
-provider to the app app.add_providers(provider) if __name__ == "__main__": #
-Start the server uvicorn.run(app) ``` ### Custom search parameters Custom
+An ASGI [FHIR](https://hl7.org/fhir/) API framework built on top of [FastAPI]
+(https://fastapi.tiangolo.com) and [FHIR Resources](https://pypi.org/project/
+fhir.resources/). Supports FHIR sequences: * [STU (v3.0.2)](https://hl7.org/
+fhir/STU3/) * [R4 (v4.0.1)](https://hl7.org/fhir/R4/) * [R4B (v4.3.0)](https://
+hl7.org/fhir/R4B/) * [R5 (v5.0.0)](https://hl7.org/fhir/R5/) ## Installation
+```bash pip install fhirstarter ``` ## Features * Automatic, standardized API
+route creation * Automatic validation of inputs and outputs through the use of
+FHIR Resources Pydantic models * Automatically-generated capability statement
+that can be customized, and a capability statement API route * An exception-
+handling framework that produces FHIR-friendly responses (i.e.
+OperationOutcomes) * Automatically-generated, integrated documentation
+generated from the FHIR specification * Custom search parameters for search
+endpoints ### Disclaimer FHIRStarter was built based on the business needs of
+[Canvas Medical](https://www.canvasmedical.com). At any point in time, it may
+not be broadly applicable to the industry at large. Canvas Medical open-sourced
+the project so that it can be used by healthcare software developers whose
+needs it might also meet. Ongoing support and development will be based on the
+business needs of Canvas Medical. ## Background FHIRStarter uses a provider-
+decorator pattern. Developers can write functions, or handlers, that implement
+FHIR interactions -- such as create, read, search-type, and update -- and plug
+them into the framework. FHIRStarter then automatically creates FHIR-compatible
+API routes from these developer-provided functions. FHIR interactions that are
+supplied must use the resource classes defined by the [FHIR Resources](https://
+pypi.org/project/fhir.resources/) Python package, which is a collection of
+Pydantic models for FHIR resources. In order to stand up a FHIR server, all
+that is required is to create a FHIRStarter and a FHIRProvider instance,
+register a FHIR interaction with the provider, add the provider to the
+FHIRStarter instance, and pass the FHIRStarter instance to an ASGI server. ##
+Usage ### Currently-supported functionality FHIRStarter supports create, read,
+search-type, and update endpoints across all FHIR resource types, and will
+automatically generate the `/metadata` capabilities statement endpoint.
+Handlers can be written as coroutines with `async/await` syntax, or as plain
+functions. FastAPI supports both, as does FHIRStarter. ### Configuration for
+specific FHIR sequences FHIRStarter will work out of the box as an R5 server.
+If a different sequence is desired, it must be specified with an environment
+variable: ```shell FHIR_SEQUENCE="R4B" ``` The latest version of the [FHIR
+Resources](https://pypi.org/project/fhir.resources/) package only supports FHIR
+STU3, R4B, and R5. FHIR R4 is supported by an earlier version. Because of this,
+if a developer desires to use FHIR R4, then the developer must pin version
+**6.4.0** of fhir.resources in their project. FHIRStarter will check the
+version of fhir.resources against the specified FHIR version in the environment
+variable to ensure that they are compatible. Model imports are also affected by
+which version of fhir.resources is installed. For STU3 and R4B, model imports
+will look like this: ```python from fhir.resources.STU3.patient import Patient
+``` ```python from fhir.resources.R4B.patient import Patient ``` For R4 and R5,
+model imports will look like this: ```python from fhir.resources.patient import
+Patient ``` ### Example A detailed example is available here: [example.py]
+(https://github.com/canvas-medical/fhirstarter/blob/main/fhirstarter/scripts/
+example.py). ```python import uvicorn from fhir.resources.fhirtypes import Id
+from fhir.resources.patient import Patient from fhirstarter import
+FHIRProvider, FHIRStarter, InteractionContext from fhirstarter.exceptions
+import FHIRResourceNotFoundError # Create the app app = FHIRStarter() # Create
+a provider provider = FHIRProvider() # Register the patient read FHIR
+interaction with the provider @provider.read(Patient) async def patient_read
+(context: InteractionContext, id_: Id) -> Patient: # Get the patient from the
+database patient = ... if not patient: raise FHIRResourceNotFoundError return
+Patient( **{ # Map patient from database to FHIR Patient structure } ) # Add
+the provider to the app app.add_providers(provider) if __name__ == "__main__":
+# Start the server uvicorn.run(app) ``` ### Custom search parameters Custom
 search parameters can be defined in a configuration file that can be passed to
 the app on creation. ```toml [search-parameters.Patient.nickname] type =
 "string" description = "Nickname" uri = "https://hostname/nickname" include-in-
 capability-statement = true ``` Adding a custom search parameter via
 configuration allows this name to be used as an argument when defining a
 search-type interaction handler and also adds this search parameter to the API
 documentation for the search endpoint. ### Capability statement It is possible
@@ -85,15 +102,8 @@
 `__init__` method on the FHIRStarter class * **provider**: the `__init__`
 method on the FHIRProvider class * **handler**: the `create`, `read`,
 `search_type`, or `update` decorator used to add a handler to a provider
 Dependencies specified at the application level will be injected into all
 routes in the application. Dependencies specified at the provider level will be
 injected into all routes that are added to the application from that specific
 provider. Dependencies specified at the handler level only apply to that
-specific FHIR interaction. ## Forward compatibility At some point in the
-future, it will be necessary to support FHIR R5. How this might be supported on
-a server that continues to support R4 has not yet been determined (e.g. a
-header that specifies the version, adding the FHIR version to the URL path,
-etc.). It may be necessary to support alteration of how the URL path is
-specified through the provider construct. Currently, the FHIR version is not
-part of the URL path, so the default behavior is that an API route defined as
-`/Patient` will be an R4 endpoint.
+specific FHIR interaction.
```

