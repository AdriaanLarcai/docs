# Verification Related Methods

The following methods are available to manage verifications.

| **RequireVerification**(IDocument doc)                                                                                                                                                                                       | Checks whether a document requires verification.                     | True if verification is required, otherwise false.          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------- | ----------------------------------------------------------- |
| **RequireVerification**(int docId)                                                                                                                                                                                           | Checks whether a document requires verification.                     | True if verification is required, otherwise false.          |
| **GetVerificationsCount**(IDocument doc)                                                                                                                                                                                     | Gets the number of verifications required on the specified document. | The number of verifications.                                |
| **GetVerificationsCount**(int docId)                                                                                                                                                                                         | Gets the number of verifications required on the specified document. | The number of verifications.                                |
| **GetVerificationParameters**(IDocument doc)                                                                                                                                                                                 | Gets all the parameters that require verification.                   | A list of document parameters.                              |
| **FindVerification**(IDocument doc, IParameterDef pd, int? index = null)                                                                                                                                                     | Try to find a verification item.                                     | The verification item and corresponding document parameter. |
| **FindVerification**(IDocument doc, int pdId, int? index = null)                                                                                                                                                             | Try to find a verification item.                                     | The verification item and corresponding document parameter. |
| **FindVerification**(int docId, int pdId, int? index = null)                                                                                                                                                                 | Try to find a verification item.                                     | The verification item and corresponding document parameter. |
| **FindVerification**(IDocumentParameter parameter)                                                                                                                                                                           | Try to find a verification item for a document parameter.            | The verification item.                                      |
| **FindVerification**(int? parameterId)                                                                                                                                                                                       | Try to find a verification item for a document parameter.            | The verification item.                                      |
| **FindVerifications**(IDocumentParameter parameter)                                                                                                                                                                          | Try to find a verification item for a document parameter.            | The verification item.                                      |
| **FindVerifications**(int? parameterId)                                                                                                                                                                                      | Try to find a verification item for a document parameter.            | The verification item.                                      |
| **FindVerifications**(int? parameterId, VerificationType? type, VerificationStatus? status, string profider = null, string valuefilter = null, string infofilter = null, DateTime? fromDate = null, DateTime? toDate = null) | Try to find a verification item for a document parameter.            | The verification item.                                      |
| **FindVerification**(int? parameterId, VerificationType? type, VerificationStatus? status, string profider = null, string valuefilter = null, string infofilter = null, DateTime? fromDate = null, DateTime? toDate = null)  | Try to find a verification item for a document parameter.            | The verification item.                                      |
| **AddVerification**(IVerification v, string result, string info = null)                                                                                                                                                      | Add a verification item to a document parameter.                     | The verification item.                                      |
| **AddVerification**(IVerification v, VerificationStatus status, string result, string info = null)                                                                                                                           | Add a verification item to a document parameter.                     | The verification item.                                      |