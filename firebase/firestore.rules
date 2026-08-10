import type { Timestamp } from 'firebase/firestore'

/**
 * Firestore type definitions.
 * 
 * These types must stay in sync with:
 *   - src/lib/firebase/firestore.ts  (typed collection exports)
 *   - firebase/firestore.rules       (security rules)
 *   - docs/FIRESTORE-SCHEMA.md       (schema documentation)
 *
 * When adding a new collection, use the /firebase-collection skill.
 */

export interface UserProfile {
  uid: string
  email: string
  displayName?: string
  photoURL?: string
  createdAt: Timestamp | string
  updatedAt: Timestamp | string
}

export type CreateUserProfileInput = Omit<UserProfile, 'createdAt' | 'updatedAt'>

export interface Note {
  id: string
  title: string
  content: string
  userId: string
  createdAt: Timestamp | string
  updatedAt: Timestamp | string
  _schemaVersion: 1
}
