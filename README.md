# marcscore

Using pymarc, this scores the quality of MARC records and returns the score along with OCLC number, title, ISSNs, and dates. It's useful for narrowing down batch searches of ISSNs where there is title duplication in the results.

The program also removes:
-Records reported for deletion
-Non-English language cataloging
-Encoding level 3
-Records where the first date begins with "0"
-Records that are not encoded "o" in the Form.

Result:

online serial | on1011201652 | 4 | Ultramicroscopy. | 0304-3991 (Print) | None | None | 1975 | 9999
online serial | ocm39196475\ | 18 | Ultramicroscopy. | 1879-2723 | 0304-3991 | None | 1975 | 9999
online serial | ocn776712731 | 0 | Ultramicroscopy | 1879-2723 | 0304-3991 | None | uuuu | uuuu
