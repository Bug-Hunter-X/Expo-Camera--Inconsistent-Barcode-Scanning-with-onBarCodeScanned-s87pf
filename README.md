# Expo Camera Barcode Scanning Inconsistency

This repository demonstrates a bug in Expo's Camera API where the `onBarCodeScanned` callback function does not always trigger when a barcode is scanned.  The issue is particularly noticeable in low-light environments or with certain barcode types.

## Bug Reproduction

1. Clone this repository.
2. Run `npm install`.
3. Run `expo start`.
4. Point the camera at a barcode.
5. Observe that the `onBarCodeScanned` callback may not fire consistently.

## Solution

The provided solution improves barcode detection reliability by incorporating additional processing steps and configuration options within the `Camera` component. The solution also handles potential errors more gracefully and provides more helpful console logs to aid debugging. 